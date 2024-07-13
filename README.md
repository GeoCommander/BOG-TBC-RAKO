**საქართველოს ბანკი:**
GE06BG0000000355227700

----------------------

**TBC ბანკი:**
GE36TB7708036020100004


# Bank Account Redirect

Click the buttons below to copy the respective bank account details to your clipboard.

### **საქართველოს ბანკი:**
<button id="copyButton1" onclick="copyToClipboard('bankData1')">Copy Bank Account 1 Details</button>
<p id="bankData1" style="display: none;">GE06BG0000000355227700</p>

### **TBC ბანკი:**
<button id="copyButton2" onclick="copyToClipboard('bankData2')">Copy Bank Account 2 Details</button>
<p id="bankData2" style="display: none;">GE36TB7708036020100004</p>

<script>
function copyToClipboard(elementId) {
    var copyText = document.getElementById(elementId).innerText;
    navigator.clipboard.writeText(copyText).then(function() {
        alert("Bank details copied to clipboard!");
    }, function(err) {
        console.error("Could not copy text: ", err);
    });
}
</script>
