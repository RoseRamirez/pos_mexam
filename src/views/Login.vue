<template>
    <div class="flex-parent rcorners2" >
        
        <div class="flex-child">
            <h4>LOGIN</h4>
            <label>Username</label>
            <input type="text" placeholder="" class="flex-items rcorners2">
            <label>Password</label>
            <input type="text" placeholder="" class="flex-items rcorners2">
            <br>
            <a href="/home"><button class="flex-items rcorners2">LOGIN</button></a>
        </div>
    </div>
</template>

<style >
body{
    background: rgb(48, 192, 120);
     margin: 0;
      padding: 0;
      height: 100%;
      box-sizing: border-box;
      background-size: cover;
      background-position: center;
      background-attachment: fixed;
      background-repeat: no-repeat;
      width: auto;
}
.flex-child{
        font-family: Verdana, Geneva, Tahoma, sans-serif;
        width: 300px;
        border: 0px solid #050505;
        border-radius: 15px;
        box-shadow:0 10px 6px -6px black;
        background-color: #ffffff;
        margin: auto;
        margin-top: 180px;
        padding-top: 20px;
        padding-bottom: 20px;
        justify-content: center;
        flex-direction: column;
        display: flex;
        align-items: center;
        text-align: center;
        font-weight: bolder;
        font-size: 30px;
}

label{
    font-weight: bold;
    font-size: 15px;
    padding-bottom: 0px;
    padding-top: 5px;
}

.flex-items{
    justify-content: center;
    flex-direction: column;
    align-items: center;
    display: flex;
    width: 80%;
    padding-top: 10px;
    margin-top: 5px;   
    box-shadow:0 10px 6px -6px rgb(231, 226, 226);
}

button{
    font-family: Verdana, Geneva, Tahoma, sans-serif;
    font-weight: bolder;
    color: rgb(251, 251, 255);
    background-color: rgb(56, 55, 55);
    border: 3px solid;
    border-radius: 10px;
    padding: 10px;

}
</style>
