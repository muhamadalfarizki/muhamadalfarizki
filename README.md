- 👋 Hi, I’m @muhamadalfarizki
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
muhamadalfarizki/muhamadalfarizki is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
imageoutput=true&script=spaceships-logo&text=",
"https://flamingtext.com/net-fu/proxy_form.cgi?imageoutput=true&script=spider-men-logo&text=",
"https://flamingtext.com/net-fu/proxy_form.cgi?imageoutput=true&script=wrestler-logo&text="
]
    return Flam
}

global.rpg = {
    emoticon(string) {
        string = string.toLowerCase()
        let emot = {
            Fox: "ðŸ¦Š",
            agility: "ðŸ¤¸â€â™‚ï¸",
            anggur: "ðŸ‡",
            apel: "ðŸŽ",
            aqua: "ðŸ¥¤",
            arc: "ðŸ¹",
            armor: "ðŸ¥¼",
            bank: "ðŸ¦",
            batu: "ðŸ§±",
            berlian: "ðŸ’Ž",
            bibitanggur: "ðŸ‡",
            bibitapel: "ðŸŽ",
            bibitjeruk: "ðŸŠ",
            bibitmangga: "ðŸ¥­",
            bibitpisang: "ðŸŒ",
            botol: "ðŸ¾",
            bow: "ðŸ¹",
            bull: "ðŸƒ",
            cat: "ðŸˆ",
            centaur: "ðŸŽ ",
            chicken: "ðŸ“",
            coal: "âš±ï¸",
            common: "ðŸ“¦",
            cow: "ðŸ„",
            crystal: "ðŸ”®",
            darkcrystal: "â™ ï¸",
            diamond: "ðŸ’Ž",
            dog: "ðŸ•",
            dragon: "ðŸ‰",
            eleksirb: "ðŸ§ª",
            elephant: "ðŸ˜",
            emasbatang: "ðŸª™",
            emasbiasa: "ðŸ¥‡",
            emerald: "ðŸ’š",
            exp: "âœ‰ï¸",
            fishingrod: "ðŸŽ£",
            foodpet: "ðŸ±",
            fox: "ðŸ¦Š",
            gardenboc: "ðŸ—³ï¸",
            gardenboxs: "ðŸ“¦",
            gems: "ðŸ€",
            giraffe: "ðŸ¦’",
            gold: "ðŸ‘‘",
            griffin: "ðŸ¦’",
            health: "â¤ï¸",
            healtmonster: "â¤â€ðŸ”¥",
            horse: "ðŸŽ",
            intelligence: "ðŸ§ ",
            iron: "â›“ï¸",
            jeruk: "ðŸŠ",
            kaleng: "ðŸ¥«",
            kardus: "ðŸ“¦",
            kayu: "ðŸªµ",
            ketake: "ðŸ’¿",
            keygold: "ðŸ”‘",
            keyiron: "ðŸ—ï¸",
            knife: "ðŸ”ª",
            koinexpg: "ðŸ‘›",
            kucing: "ðŸˆ",
            kuda: "ðŸŽ",
            kyubi: "ðŸ¦Š",
            legendary: "ðŸ—ƒï¸",
            level: "ðŸ§¬",
            limit: "ðŸŒŒ",
            lion: "ðŸ¦",
            magicwand: "âš•ï¸",
            makanancentaur: "ðŸ¥—",
            makanangriffin: "ðŸ¥™",
            makanankyubi: "ðŸ—",
            makanannaga: "ðŸ–",
            makananpet: "ðŸ¥©",
            makananphonix: "ðŸ§€",
            mana: "ðŸª„",
            mangga: "ðŸ¥­",
            money: "ðŸ’µ",
            mythic: "ðŸ—³ï¸",
            mythic: "ðŸª„",
            naga: "ðŸ‰",
            pancingan: "ðŸŽ£",
            pet: "ðŸŽ",
            petFood: "ðŸ–",
            phonix: "ðŸ¦…",
            pickaxe: "â›ï¸",
            pisang: "ðŸŒ",
            pointxp: "ðŸ“§",
            potion: "ðŸ¥¤",
            rock: "ðŸª¨",
            rubah: "ðŸ¦Š",
            sampah: "ðŸ—‘ï¸",
            serigala: "ðŸº",
            snake: "ðŸ",
            stamina: "âš¡",
            strength: "ðŸ¦¹â€â™€ï¸",
            string: "ðŸ•¸ï¸",
            superior: "ðŸ’¼",
            sword: "âš”ï¸",
            tiger: "ðŸ…",
            tiketcoin: "ðŸŽŸï¸",
            trash: "ðŸ—‘",
            umpan: "ðŸª±",
            uncommon: "ðŸŽ",
            upgrader: "ðŸ§°",
            wood: "ðŸªµ"
        }
        let results = Object.keys(emot).map(v => [v, new RegExp(v, "gi")]).filter(v => v[1].test(string))
        if (!results.length) return ""
        else return emot[results[0][0]]
    }
}


//------ JANGAN DIUBAH -----
let file = fileURLToPath(import.meta.url)
watchFile(file, () => {
  unwatchFile(file)
  console.log(chalk.redBright("Update 'config.js'"))
  import(`${file}?update=${Date.now()}`)
})
//=========/===
