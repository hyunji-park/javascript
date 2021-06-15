<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <script>
        function parent(){
            var a = 1;
            var b = 2;

            function child(){
            var c = 3;
            var d = 4;
            console.log(b);
            //내부 함수에 외부함수내용을 참조해야만 스코프 생성
            console.log(c);
            console.log(d);
        }
        return child;
        }
        var c = parent;
        console.dir(c);
    </script>
</body>
</html>
