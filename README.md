# WaferText.js

**warning this code was deprecated**

WaferText.js is a rich textarea which is completely free and easy to use !
This is the first version there may be some errors

**How to apply**

include waferText.js and waferStyle.css in header.

     <link rel="stylesheet" href="waferStyle.css">
     <script src="waferText.js"></script>

waferText.js declaration to div.

      <div id="content"></div>
      
      <script>
        new WaferText('#content');
      </script>

Sample Results : 👍

![Sample Results](https://user-images.githubusercontent.com/80049379/133304213-fdbb4d8a-7d0d-4e65-989b-748c811f5005.png)

With custom toolbar :

    new WaferText('#content').newToolBar(['link', 'bold', 'headingSelection']);

Result :

![Sample Custom toolbar](https://user-images.githubusercontent.com/80049379/133305504-149dd366-ac89-4d50-8c4f-87c57c7caed4.png)

list of items :

* headingSelection
* bold
* Italic
* underLine
* link
* justifyLeft
* justifyCenter
* justifyRight
* dotList
* numList
* textIndentLeft
* textIndentRight
* quote
* image
* video
* undo
* redo

To get content text with form.

  Create HTML form :

     <form method="post" action='data.php'>
        <div id="content"></div>
        <br/>
        <button type="submit" class="submit-btn">submit</button>
    </form>

Script :

    new WaferText('#content').newToolBar(['headingSelection', 'link', 'bold']).getText();

  data.php :

    echo $_POST[ 'WaferData' ];

Report any problem here ! 💯
