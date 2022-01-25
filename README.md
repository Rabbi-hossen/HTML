<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Day_1</title>
    <!-- google font -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Pacifico&display=swap" rel="stylesheet">

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Pacifico&display=swap" rel="stylesheet">

<!-- logo -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
</head>
<style>
    /* google font */
    body{
        font-family: 'Pacifico', cursive;
        font-family: 'Pacifico', cursive;
    }
    /* price table */
  
    .columns{
        float: left;
        width: 33.3%;
        padding: 8px;
        box-sizing: border-box;
    }

    .price{
        list-style-type: none ;
        border: 1px solid #eee;
        margin: 0;
        padding: 0 ;
        -webkit-transition:0.3s ;
        transition: 0.3s;
    }
    .price:hover{
        box-shadow: 0 8px 12px 0 rgba(0,0,0,0.2);
    }
    .price .header{
        background-color: #111 ;
        color: white;
        font-size: 25px;
    }
    .price li{
        border-bottom: 1px solid #eee;
        padding: 20px;
        text-align: center;
    }
     .price .red{
        background-color: #e9eb6e;
        font-size: 20px;
    }
    .price .grey{
        background-color: #eee;
        font-size: 20px;
    } 
   /*  .price .grey {
 background-color: #eee;
  font-size: 25px; 
} */
.button {
  background-color: #04AA6D;
  border: none;
  color: white;
  padding: 10px 25px;
  text-align: center;
  text-decoration: none;
  font-size: 20px;
}
    @media only screen and (max-width: 600px) {
  .columns {
    width: 100%;}}
    
    /* contact form */
    input [ type=text ], select, textarea{

width: 100%;
padding: 12px;
border: 1px solid #ccc;
border-radius: 4px;
box-sizing: border-box;
margin-top: 6px;
margin-bottom: 16px;
resize: vertical;

} 
input[type=submit]{
    background-color: #04aa6d;
    color: white;
    padding: 25px ;
    border: none;
    border-radius: 10px;
    cursor: pointer;
    
}


input[type=submit]:hover{
    background-color: rgb(238, 231, 231);
}
.container{
    border-radius: 5px;
    background-color: #ddc5c5;
    padding: 20px;
}
h1 {text-align: center;}

/* striped table */
table{
    border-collapse: collapse;
    width: 100%;
}
th,td{
    text-align: left;
    padding: 8px;

}
tr:nth-child(even){
    background-color: #d6f7eb;
}
/* image */
.img{
    
        
}
/* logo */

.fa{
    padding: 20px;
  font-size: 30px;
  width: 50px;
  text-align: center;
  text-decoration: none;
  margin: 2px 10px;
}
.fa:hover {
    opacity: 0.7;
}
.fa-facebook{
    background: #3B5998;
  color: white;
}
.fa-twitter{
    background: #55ACEE;
  color: white;
}
.fa-google {
  background: #dd4b39;
  color: white;
}
</style>

                 <!-- starting html portion -->
<body>
    <!-- price table -->
    <div>
    <h1>Price Table</h1>
    
    <div class="columns">
        <ul class="price">
            <li class="header">Basic</li>
            <li>10 GB Storage</li>
            <li>10 Emails</li>
            <li>10 Domail</li>
            <li class="red">$9.99</li>
            <li class="grey"><a href="#" class="button">Sign Up</a></li>
        </ul>
    </div>
    <div class="columns">
        <ul class="price">
            <li class="header">Pro</li>
            <li>25 GB Storage</li>
            <li>25 Emails</li>
            <li>25 Domail</li>
            <li class="red">$24.99</li>
            <li class="grey"><a href="#" class="button">Sign Up</a></li>
        </ul>
    </div>
    <div class="columns">
        <ul class="price">
            <li class="header">Premium</li>
            <li>50 GB Storage</li>
            <li>50 Emails</li>
            <li>50 Domail</li>
            <li class="red">$39.99</li>
            <li class="grey"><a href="#" class="button">Sign Up</a></li>
        </ul>
    </div>
</div>
<br>
<br><br><br><br>
    <!-- contact form -->
        <h1 >contact form </h1>
    <div class="container">
        <form action="backend.php">
     <label for="fname">First Name</label>
     <input type="text" id="fname" name="firstname" placeholder="your first name..." >
      <br><br>
     <div>
     <label for="lname">Last Name</label>
     <input type="text" name="lastname" id="lname" placeholder="Your last name...">
    </div> 
    <br>
     <div>
     <label for="email">Mailing Address</label>
     <input type="text" name="mail" id="email" placeholder="your gamil address...">
    </div>
    <br>
    phone Number <input type="text" name="phn" placeholder="+8801..." >
    
    <br>
    <br>
     <label for="country">country name </label>
     <select name="country" id="country">
    
      <option value="BD">Bangladesh</option>
      <option value="IND">India</option>
      <option value="JRN">Jerman</option>
      <option value="cina">China</option>

     </select>

     <label for="subject">Subject</label>
     <textarea name="subject" id="subject" placeholder="Write something..." cols="30" rows="10" ></textarea>
  
     <input type="submit" value="submit">
     

    </form>

    </div>

          <!-- striped table -->
<div>
    <h1>Striped Table for player Ranking </h1>
<table>
       <tr>
           <th>Name</th>
           <th>Age</th>
           <th>Rank</th>
       </tr>
       <tr>
           <td>Hafizur</td>
           <td>52</td>
           <td>1</td>
       </tr>
        <tr>
            <td>sakib</td>
            <td>22</td>
            <td>2</td>
        </tr>
        <tr>
            <td>Rabbi</td>
            <td>22</td>
            <td>3</td>
        </tr>
        <tr>
            <td>Shoykot</td>
            <td>13</td>
            <td>4</td>
        </tr>
</table>


</div>
<div class="img">
    <img src="https://cdn.pixabay.com/photo/2018/11/17/22/15/trees-3822149_960_720.jpg" alt="photo">
</div>
<!-- some  logo -->
<div>
<h1>logo</h1>
<a href="#" class="fa fa-facebook"></a>
<a href="#" class="fa fa-twitter"></a>
<a href="#" class="fa fa-google"></a>

</div>

    
</body>
</html>
