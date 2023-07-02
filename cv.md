# Maryna Verbovska

## Frontend Developer

![photo](ava.jpeg "Photo")

### Contact information:

- Contact phone: +380981218919
- E-mail: verbovskaya.freelance@gmail.com
- Telegram: [@maryna_zaitseva](адрес "https://t.me/maryna_zaitseva")
- Linkedn: [@maryna_zaitseva](адрес "https://t.me/maryna_zaitseva")

### About myself:

Hello, my name is Maryna Verbovska! I am a Front-end developer. I have knowledge of HTML,CSS,JS,React and Bootstrap. I am looking forward to working in teams as well as individually. I could speak English (B1), German(B1), Russian(Native) and Ukrainian(Native)

### Skills and Proficiency:

| Hard skills:             |   Soft skills   |
| ------------------------ | :-------------: |
| HTML, CSS and JS         |     Empathy     |
| Bootstrap                |  Communication  |
| Responsive/mobile design |    Ambition     |
| Javascript               | Industriousness |
| Adobe Photoshop, Figma   |    Teamwork     |

### Code example:

#### Tic-tac-toe game (JS)

` let area = document.getElementById('area');
let cell = document.getElementsByClassName('cell');
let currentPlayer = document.getElementById('curPlyr');`

`let player = "x";
let stat = {
'x': 0,
'o': 0,
'd': 0
}`
`let winIndex = [
[1,2,3],
[4,5,6],
[7,8,9],
[1,4,7],
[2,5,8],
[3,6,9],
[1,5,9],
[3,5,7]
];`

`for(let i = 1; i <= 9; i++) {
area.innerHTML += "<div class='cell' pos=" + i + "></div>";
}

for (let i = 0; i< cell.length; i++) {
cell[i].addEventListener('click', cellClick, false);
}
`
`function cellClick() {
let data = [];

    if(!this.innerHTML) {
        this.innerHTML = player;
    } else {
        alert("Ячейка занята");
        return;
    }

    for(let i in cell){
        if(cell[i].innerHTML == player){
            data.push(parseInt(cell[i].getAttribute('pos')));
        }
    }

    if(checkWin(data)) {
        stat[player] += 1;
        restart("Выграл: " + player);
    }else {
        let draw = true;
        for(let i in cell) {
            if(cell[i].innerHTML == '') draw = false;
        }
        if(draw) {
            stat.d += 1;
            restart("Ничья");
        }
    }

    player = player == "x" ? "o" : "x";
    currentPlayer.innerHTML = player.toUpperCase();

}
`
`function checkWin(data) {
for(let i in winIndex) {
let win = true;
for(let j in winIndex[i]) {
let id = winIndex[i][j];
let ind = data.indexOf(id);

            if(ind == -1) {
                win = false
            }
        }
        if(win) return true;
    }
    return false;

}
`
`function restart(text) {
alert(text);
for(let i = 0; i < cell.length; i++) {
cell[i].innerHTML = '';
}
updateStat();
}
`
`function updateStat() {
document.getElementById('sX').innerHTML = stat.x;
document.getElementById('sO').innerHTML = stat.o;
document.getElementById('sD').innerHTML = stat.d;
}`
`

### Work experience:

|         Positions:         |         Years          |                                  Responsibilities                                  |
| :------------------------: | :--------------------: | :--------------------------------------------------------------------------------: |
|     Internet Marketer      |  Aug 2021 - Apr 2022   |                 \* Creation of the site on Wordpress (Elementor),                  |
|                            |                        |                           \* Creation of website design,                           |
|                            |                        |                    \* Connection / transfer of hosting, domain                     |
| :------------------------: | :--------------------: | :--------------------------------------------------------------------------------: |
|         Freelancer         |  Jan 2019 - Jul 2021   |            \* Creation of sites on Tilda, Wordpress, Octstore/OpenCart             |
|                            |                        |                           \* Creation of website design                            |
|                            |                        |  \* Setting up and connecting Google Analytics, Google Ads, Google Search Console  |
|                            |                        |                    \* Connection / transfer of hosting, domain                     |
|                            |                        |                        \* Setting up contextual advertising                        |
| :------------------------: | :--------------------: | :--------------------------------------------------------------------------------: |
|    Marketing Assistant     |  Apr 2018 - Jan 2019   |                         \* Created layouts for web pages;                          |
|                            |                        |              \* Preparation of technical specifications for designers              |
| :------------------------: | :--------------------: | :--------------------------------------------------------------------------------: |

### Skills and Proficiency:

- KNUE (marketing)
- Epam for Switchers (Frontend)
- WayUp "Web Development"
- WayUp "Javascript"
- Course I. Petrichenko "Web Development"(in progress)
- Course I. Petrichenko "Javascript/React"(in progress)
- RS Schools Course «JavaScript/Front-end. Stage 0» (in progress)

### Languages:

---

- Russian (native);
- Ukrainian (native);
- English (B1);
- German (B1);
