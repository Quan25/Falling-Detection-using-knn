# Falling-Detection-using-knn
  This project uses K-Nearest Neighbor(KNN) algorithm in machine learning to help
  predict Falling

  use Python to implement the application of using kNN to predict falling because:

  - Most mobile devices are equipped with different kind of sensors.
  - We can use the data sent from Gyroscope and Accelerometer sensors to categorize
  any motion:
    - 3 numbers from Accelerometer sensor
    - 3 numbers from Accelerometer sensor

  - This is the training data and the test data:

  <style type="text/css">
  .tg  {border-collapse:collapse;border-spacing:0;}
  .tg td{font-family:Arial, sans-serif;font-size:14px;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;border-color:black;}
  .tg th{font-family:Arial, sans-serif;font-size:14px;font-weight:normal;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;border-color:black;}
  .tg .tg-c3ow{border-color:inherit;text-align:center;vertical-align:top}
  .tg .tg-dxjg{color:#fe0000;border-color:#fe0000;text-align:center;vertical-align:top}
  .tg .tg-s256{color:#fe0000;border-color:#fe0000;text-align:left;vertical-align:top}
  .tg .tg-kwiq{color:#000000;border-color:inherit;text-align:left;vertical-align:top}
  .tg .tg-0lax{text-align:left;vertical-align:top}
  .tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
  </style>
  <table class="tg">
    <tr>
      <th class="tg-0lax" colspan="3">Accelerometer Data</th>
      <th class="tg-kwiq" colspan="3">Gyroscope Data</th>
      <th class="tg-kwiq">Fall (+), Not (-)</th>
    </tr>
    <tr>
      <td class="tg-0pky">x1</td>
      <td class="tg-0pky">y1</td>
      <td class="tg-0pky">z1</td>
      <td class="tg-0pky">x2</td>
      <td class="tg-0pky">y2</td>
      <td class="tg-0pky">z2</td>
      <td class="tg-c3ow">+/-</td>
    </tr>
    <tr>
      <td class="tg-0pky">1</td>
      <td class="tg-0pky">2</td>
      <td class="tg-0pky">3</td>
      <td class="tg-0pky">2</td>
      <td class="tg-0pky">1</td>
      <td class="tg-0pky">3</td>
      <td class="tg-c3ow">-</td>
    </tr>
    <tr>
      <td class="tg-0pky">2</td>
      <td class="tg-0pky">1</td>
      <td class="tg-0pky">3</td>
      <td class="tg-0pky">3</td>
      <td class="tg-0pky">1</td>
      <td class="tg-0pky">2</td>
      <td class="tg-c3ow">-</td>
    </tr>
    <tr>
      <td class="tg-0pky">1</td>
      <td class="tg-0pky">1</td>
      <td class="tg-0pky">2</td>
      <td class="tg-0pky">3</td>
      <td class="tg-0pky">2</td>
      <td class="tg-0pky">2</td>
      <td class="tg-c3ow">-</td>
    </tr>
    <tr>
      <td class="tg-0pky">2</td>
      <td class="tg-0pky">2</td>
      <td class="tg-0pky">3</td>
      <td class="tg-0pky">3</td>
      <td class="tg-0pky">2</td>
      <td class="tg-0pky">1</td>
      <td class="tg-c3ow">-</td>
    </tr>
    <tr>
      <td class="tg-0pky">6</td>
      <td class="tg-0pky">5</td>
      <td class="tg-0pky">7</td>
      <td class="tg-0pky">5</td>
      <td class="tg-0pky">6</td>
      <td class="tg-0pky">7</td>
      <td class="tg-c3ow">+</td>
    </tr>
    <tr>
      <td class="tg-0pky">5</td>
      <td class="tg-0pky">5</td>
      <td class="tg-0pky">6</td>
      <td class="tg-0pky">6</td>
      <td class="tg-0pky">5</td>
      <td class="tg-0pky">7</td>
      <td class="tg-c3ow">+</td>
    </tr>
    <tr>
      <td class="tg-0pky">5</td>
      <td class="tg-0pky">6</td>
      <td class="tg-0pky">7</td>
      <td class="tg-0pky">5</td>
      <td class="tg-0pky">7</td>
      <td class="tg-0pky">6</td>
      <td class="tg-c3ow">+</td>
    </tr>
    <tr>
      <td class="tg-0pky">7</td>
      <td class="tg-0pky">6</td>
      <td class="tg-0pky">7</td>
      <td class="tg-0pky">6</td>
      <td class="tg-0pky">5</td>
      <td class="tg-0pky">6</td>
      <td class="tg-c3ow">+</td>
    </tr>
    <tr>
      <td class="tg-s256">7</td>
      <td class="tg-s256">6</td>
      <td class="tg-s256">5</td>
      <td class="tg-s256">5</td>
      <td class="tg-s256">6</td>
      <td class="tg-s256">7</td>
      <td class="tg-dxjg">??</td>
    </tr>
  </table>


  </table>

  ## tools used for this project
  - Jupyter Python Notebook
  - Pandas library
  - Numpy library
  - Sklearn library

  ## Steps of this project
    - step 1:
      - load the data using pandas
   - step 2:
      - Split the data into training and testing dataset
    - step 3:
      - Accuracy test based on the give training and testing dataset
    -step 4:
      - feed the red marked data into the model and do the prediction
