# hw5

- 競賽題1:
```CSS
const apple = () => {
  const a = 1;
  const b = 2;
  const c = 3;
  console.log(`a是:${a} b是:${b} c是:${c}`)
};
apple();
```
- 競賽題2:
```CSS
function print(input) {
  if (input === 0) {
    console.log("輸入的是0");
  } else if (input > 0) {
    console.log("輸入的是正數");
  } else {
    console.log("輸入的是負數");
  }
}
print(0);
```
- 競賽題3:
```CSS
<!DOCTYPE html>
<html lang="zh-Hant">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <style>
        .mypage {
            color: red;
        }

        @media screen and (max-width: 1023px) {
            .mypage {
                color: blue;
            }
        }
    </style>
</head>

<body>

    <p class="mypage">html try</p>

</body>

</html>

- 競賽題4:
```CSS
<!DOCTYPE html>
<html lang="zh-Hant">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <style>
        #img {
            display: none;
        }
    </style>
</head>

<body>

    <img id='img' src="https://fakeimg.pl/150x130">
    <button id='botton1'>顯示圖片</button>
    <button id='botton2'>隱藏圖片</button>

    <script>
        const img = document.getElementById('img');
        const botton1 = document.getElementById('botton1');
        const botton2 = document.getElementById('botton2');

        botton1.addEventListener('click', function() {
            img.style.display = 'block';
        });

        botton2.addEventListener('click', function() {
            img.style.display = 'none';
        });
    </script>
</body>

</html>

```
- 競賽題5:
```CSS
<!DOCTYPE html>
<html lang="zh-Hant">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <style>
        #label {
            font-size: 24px;
            margin-bottom: 10px;
        }
    </style>
</head>

<body>

    <div id='label'>我的網頁</div>
    <button id='botton1'>黑</button>
    <button id='botton2'>藍</button>

    <script>
        const label = document.getElementById('label');
        const botton1 = document.getElementById('botton1');
        const botton2 = document.getElementById('botton2');

        botton1.addEventListener('click', function () {
            label.style.color = 'black';
        });

        botton2.addEventListener('click', function () {
            label.style.color = 'blue';
        });
    </script>
    
</body>

</html>
```

- 競賽題6:
```CSS
function printTree(treeHeight, treeGap) {
  let result = "";
  const maxStar = 1 + (treeHeight - 1) * treeGap;

  for (let i = 0; i < treeHeight; i++) {
    const stars = 1 + i * treeGap;
    const dashes = (maxStar - stars) / 2;
    const levelStr = "-".repeat(dashes) + "*".repeat(stars) + "-".repeat(dashes);
    result += levelStr + "\n";
  }
  return result;
}

const treeHeight = 5;
const treeGap = 2; 
console.log(printTree(treeHeight, treeGap));
```
