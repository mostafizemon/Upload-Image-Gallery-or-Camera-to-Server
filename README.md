Here the php Code:
<?php
$image64=$_POST['image'];
$decodeimage=base64_decode($image64);
$filename=uniqid().'.jpg';
$filepath='image/'.$filename;

if (file_put_contents($filepath,$decodeimage)){
    echo "File upload successfully";
}
else{

}
?>
