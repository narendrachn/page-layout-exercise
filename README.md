# Page Layout Exercise

Create a 2-column page layout using floats. 

1. Clone this repository onto your local computer.
2. In VSCode, structure the content in index.html following the diagram below: <br>
![image](images/semantic-html.png)<br>
3. Write the CSS in the external stylesheet to make the HTML look like the image below, where the nav's width is 30%:<br>
![image](images/result.png)

Tip: You will need to use the CSS box-sizing property and the CSS calc function to make this work.
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Page Layout Exercise</title>
    <link rel="stylesheet" href="style.css" />
  </head>

  <body>
    <div class="wrapper">
      <header><h1>Page Layout Example</h1></header>

      <nav class="hint">
        <ul>
          <li>Home</li>
          <li>Page 1</li>
          <li>Page 2</li>
        </ul>
      </nav>
      <main class="hint">
        This is a sample 2-column page layout using floats. It includes a
        header, a vertical nav next to the main content and a footer. You will
        need to use the CSS box-sizing property and the CSS calc function to
        make this work.
      </main>
      <footer>Copyright &#169;2022</footer>
    </div>
  </body>
</html>


css
/* COLOURS 

 dark purple: #2E1345;
 light blue: #ccccff;
 beige: #F1F0F6;

 */

body {
    background-color: #2E1345;
 }
 .wrapper{
    width: 960px;
    margin: 40px auto;
 }
header {
    color: white;
    font-size: 35px;
 }
nav{
    background-color: #ccccff;
    

    list-style-type: none;
    float: left;
    width: 33.33%;

}
main{
    box-sizing: calc(63%);
    background-color: white;
    float: right;
    width: 60%;
    padding: 100px;

}
.hint{
    box-sizing: border-box;
 
}
footer {
    color: #F1F0F6;
    text-align: center;
    clear: both;
    padding-top: 20px;
}
