# button-onclick-js-css
Как при нажатии кнопки получить блок div?

        function viewDiv(){
          document.getElementById("div1").style.display = "block";
        };
        #div1{
          display: none;
        }
        <input type="button" value="Click" onmousedown="viewDiv()">
        <div id="div1">Блок</div>



        $('.btn').click(function(){
          $(".block_with_text").fadeToggle(100);
        });  
        <script src="https://ajax.googleapis.com/ajax/libs/jquery/2.0.0/jquery.min.js"></script>
        <button class="btn">Кликни по мне</button>
        <div class="block_with_text">Lorem ipsum dolor sit amet</div>


        .text,
        input[type="checkbox"] {
          display: none;
        }

        input[type="checkbox"]:checked ~ .text {
          display: block;
        }

        /* Стилизация псевдокнопки */
        .btn {
          display: inline-block;
          margin-bottom: 4px;
          padding: 4px 8px;
          background-color: #ffffff;
          border: 1px solid #eeeeee;
          cursor: pointer;
        }
        <label for="pseudoBtn" class="btn">"Кнопка"</label>
        <input type="checkbox" id="pseudoBtn">
        <div class="text">Готовый текст</div>
