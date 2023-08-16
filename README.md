# Flecha
É um site de rede social 
<!DOCTYPE html>
<html>
<head>
    <title>Mini YouTube</title>
</head>
<body>

<h1>Mini YouTube</h1>

<input type="file" id="videoFile" accept="video/*">
<video id="videoPlayer" controls width="320" height="240"></video>

<script>
document.getElementById('videoFile').addEventListener('change', function(e) {
    var file = e.target.files[0];
    var url = URL.createObjectURL(file);
    document.getElementById('videoPlayer').src = url;
});
</script>

</body>
</html>
