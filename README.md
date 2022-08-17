# cheer-o-meter
Built in Zurich

the things you need to add to the Teachable machine template


```
<button onclick="score = 50">reset</button>
<div id="meter" style="height: 100%; width: 50%; background-color: blueviolet; transition: width 0.5s"></div>
```

```   
var score = 50
```

```
if (result.scores[1] > 0.5) {
    score -= 5
} else if (result.scores[2] > 0.5) {
    score += 5
}

score = Math.max(0, Math.min(100, score))
document.getElementById("meter").style.width = `${score}%`
```
