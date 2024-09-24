# api-1
this is the basic file of the json api of the burgers with there image you can easly use these data
Sample code for accessing the data 
 <table class="table">
      <thead>
        <tr>
          <th scope="col">id</th>
          <th scope="col">name</th>
          <th scope="col">image</th>
          <th scope="col">Desciption</th>
          <th scope="col">Price</th>
        </tr>
      </thead>
      <tbody></tbody>
    </table>
    <script>
      var tr = "";
      fetch("final.json")
        .then((response) => response.json())
        .then((data) =>
          data.forEach((currele, indx, arr) => {
            tr +=
              `<tr>
                  <td>` +
              currele.id +
              `</td>
                  <td>` +
              currele.name +
              `</td>

                 <td>
                    <img src =` +
              currele.image_url +
              `></td>
              <td>` +
              currele.description +
              `</td>
                 <td>` +
              currele.price +
              `</td>
                </tr>`;

            document.querySelector("table>tbody").innerHTML = tr;
          })
        );
    </script>
