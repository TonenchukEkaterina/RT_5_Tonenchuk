# RT_5_Tonenchuk
<html xmlns="http://www.w3.org/1999/xhtml">
 <head>    
 <title>Примеры. Добавление прямоугольника на карту.</title>
<meta http-equiv="Content-Type" content="text/html; charset=utf-8"/>  
    <!--         Подключаем API карт 2.x
         Параметры:
           - load=package.full - полная сборка;
        - lang=ru-RU - язык русский.     -->
      <script src="http://api-maps.yandex.ru/2.0/?load=package.full&lang=ru-RU"
             type="text/javascript"></script>
     <script type="text/javascript"> 
        ymaps.ready(init);  
        function init() { 
            var myMap = new ymaps.Map('map', { 
                center: [65.509389, -151.390021], 
                zoom: 8         
 }),            
                 
 myPolygon = new ymaps.Polygon([[
			[65.587925,-151.374911],
			[65.413461,-151.078287],
			[65.413757,-151.567177],			
                ]]);
  
            myMap.geoObjects.add(myPolygon)
                 .add(myPolygon); 
        }     </script> 
</head>  
<body> 
<h2>Добавление прямоугольника на карту</h2>  
<div id="map" style="width:600px;height:400px"></div> </body>  
</html>  
 
