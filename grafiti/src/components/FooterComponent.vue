<template>
<div>
<p>Email: support@shop.com</p>
</div>
</template>


  <script>
  export default {
    name: "FooterComponent",
  };
  </script>
  
  <style scoped>
  .footer {
    background-color:rgb(255, 255, 255);
    margin-top: 40px;
    color: #333;
    text-align: center;
    border-top: 1px solid #ddd;
  }
  
  .footer-content {
    display: flex;
    justify-content: center;
    gap: 80px;
    padding: 0 10%;
  }
  
ul {
    list-style: none;
    padding: 0;
    display:flex;
    gap: 80px;
  }
  
li {
    margin-bottom: 5px;
  }
  
a {
    text-decoration: none;
    color: black;
  }
  
a:hover {
    text-decoration: underline;
  }
 
  .footer-bottom {
    margin-top: 20px;
    font-size: 14px;
    color: #666;
  }
  </style>