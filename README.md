# api-1
this is the basic file of the json api of the burgers with there image you can easly use these data
Sample code for accessing the data 
 
    <script>
      var tr = "";
      fetch("https://shivammathtech.github.io/api-1/final.json")
        .then((response) => response.json("))
        .then((data) =>
          data.forEach((currele, indx, arr) => {
           console.log(currele)
          })
        );
    </script>
