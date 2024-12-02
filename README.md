# lab6Web.
<!DOCTYPE html>
<html 
<head>
    <script src=""http:ajax.googleapis.com/ajax/libs/jquery/1.10.2/jquery.min.js">
    </script>
    <script>
    $(document).ready(function(){
        $("#flip").click(function(){
            $("#panel").slideToggle("slow");
        });
    });
    </script>

    <style type="text/css">
        #panel, #flip {
            padding: 5px;
            text-align: center;
            background-color: #e5eecc;
            border: solid 1px #c3c3c3;
        }
        #panel {
            padding: 50px;
            display: none;
        }

    </style>
</head>
<body>
    <div id = "flip">Click to slide the panel down or up</div>
    <div id = "panel">Hello world!</div>
</body>
</html>

![image](https://github.com/user-attachments/assets/285198ca-8385-43ef-9931-ea2dc27f94e4)

<!DOCTYPE html>
<html>
<head>
    <script src="http://ajax.googleapis.com/ajax/libs/jquery/1.10.2/jquery.min.js">
    </script>
    <script>
    $(document).ready(function(){
        $("button").click(function(){
            var div=$("div");
            div.animate({height:'300px',opacity:'0.4'}, "slow");
            div.animate({height:'300px',opacity:'0.8'}, "slow");
            div.animate({height:'100px',opacity:'0.4'}, "slow");
            div.animate({height:'100px',opacity:'0.8'}, "slow");
        });
    });
    </script>
</head>
<body>
    <button>Start Animation</button>
    <div style="background:#98bf21;height:100px;width:100px;position:absolute;"></div>
</body>
</html>

![image](https://github.com/user-attachments/assets/f409bfa0-2a9b-44b9-b886-49d034640ffa)

<!DOCTYPE html>
<html>
<head>
    <title>Elemen yang Dapat Ditarik</title>
    <link rel="stylesheet" href="http://code.jquery.com/ui/1.10.3/themes/base/jquery-ui.css" />
    <script src="http://code.jquery.com/jquery-1.9.1.js"></script>
    <script src="http://code.jquery.com/ui/1.10.3/jquery-ui.js"></script>
    <style>
        #draggable {
            width: 125px;
            height: 125px;
            background-color: #FFF;
            text-align: center;
            padding: 1px 5px;
            border: 1px solid #AAA;
            margin: auto;
            float: left;
        }

        #containment-wrapper {
            width: 95%;
            height: 200px;
            border: 1px solid #4E4E4E;
            padding: 10px;
        }
    </style>
    <script>
        $(function() {
            $("#draggable").draggable({
                containment: "#containment-wrapper",
                scroll: false
            });
        });
    </script>
</head>
<body>
    <div id="containment-wrapper">
        <div id="draggable">
            <p>I'm contained within the box</p>
        </div>
    </div>
</body>
</html>

![image](https://github.com/user-attachments/assets/2b402953-8cc8-4ac6-8f3e-1b67cdd9e3ff)
