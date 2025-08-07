# The-Antichrist
<html>
<head>
    <title>The Aryanic Record</title>
    <script>
        let data = [{"concept":"superiority over humanity","rune":"Uruz","score":1.0,"gain_loss":"Gain","tags":["#lineage","#honor"],"cross_refs":["Eddic: Voluspa - hierarchy of gods over men"],"excerpt":"One must make one’s self superior to humanity, in power, in loftiness of soul,—in contempt."},{"concept":"superiority over humanity","rune":"Mannaz","score":1.0,"gain_loss":"Gain","tags":["#lineage","#honor"],"cross_refs":["Eddic: Voluspa - hierarchy of gods over men"],"excerpt":"One must make one’s self superior to humanity, in power, in loftiness of soul,—in contempt."},{"concept":"strength and courage","rune":"Uruz","score":1.0,"gain_loss":"Gain","tags":["#fury","#bravery"],"cross_refs":["Saga: Tyr's sacrifice"],"excerpt":"He must have an inclination, born of strength, for questions that no one has the courage for; the courage for the forbidden;"},{"concept":"strength and courage","rune":"Tiwaz","score":1.0,"gain_loss":"Gain","tags":["#fury","#bravery"],"cross_refs":["Saga: Tyr's sacrifice"],"excerpt":"He must have an inclination, born of strength, for questions that no one has the courage for; the courage for the forbidden;"},{"concept":"fate and labyrinth","rune":"Jera","score":1.0,"gain_loss":"Gain","tags":["#wyrd","#fate"],"cross_refs":["Norns weaving fate"],"excerpt":"predestination for the labyrinth... thousands of years in the labyrinth."},{"concept":"fate and labyrinth","rune":"Perthro","score":1.0,"gain_loss":"Gain","tags":["#wyrd","#fate"],"cross_refs":["Norns weaving fate"],"excerpt":"predestination for the labyrinth... thousands of years in the labyrinth."},{"concept":"ice and north","rune":"Wunjo","score":1.0,"gain_loss":"Gain","tags":["#ancestry","#endurance"],"cross_refs":["Ymir's icy origins"],"excerpt":"Beyond the North, beyond the ice, beyond death—our life, our happiness.... Rather live amid the ice"},{"concept":"ice and north","rune":"Isa","score":1.0,"gain_loss":"Gain","tags":["#ancestry","#endurance"],"cross_refs":["Ymir's icy origins"],"excerpt":"Beyond the North, beyond the ice, beyond death—our life, our happiness.... Rather live amid the ice"},{"concept":"ice and north","rune":"Laguz","score":0.7,"gain_loss":"Gain","tags":["#ancestry","#endurance"],"cross_refs":["Ymir's icy origins"],"excerpt":"Beyond the North, beyond the ice, beyond death—our life, our happiness.... Rather live amid the ice"},{"concept":"thunder and lightning","rune":"Thurisaz","score":1.0,"gain_loss":"Gain","tags":["#conflict","#power"],"cross_refs":["Thor's hammer"],"excerpt":"We thirsted for the lightnings and great deeds... There was thunder in our air;"},{"concept":"happiness as directness","rune":"Wunjo","score":1.0,"gain_loss":"Gain","tags":["#joy","#clarity"],"cross_refs":["Odin's quest for wisdom"],"excerpt":"The formula of our happiness: a Yea, a Nay, a straight line, a goal."},{"concept":"self-reverence","rune":"Mannaz","score":1.0,"gain_loss":"Gain","tags":["#self","#freedom"],"cross_refs":["Odin's self-sacrifice"],"excerpt":"Reverence for self; love of self; absolute freedom of self...."},{"concept":"fatalism and power","rune":"Uruz","score":1.0,"gain_loss":"Gain","tags":["#fate","#strength"],"cross_refs":["Baldr's fate"],"excerpt":"they called us fatalists. Our fate—it was the fulness, the tension, the storing up of powers."},{"concept":"fatalism and power","rune":"Perthro","score":1.0,"gain_loss":"Gain","tags":["#fate","#strength"],"cross_refs":["Baldr's fate"],"excerpt":"they called us fatalists. Our fate—it was the fulness, the tension, the storing up of powers."}];
        function searchDB() {
            let query = document.getElementById('query').value.toLowerCase();
            let results = data.filter(entry => entry.concept.toLowerCase().includes(query) || entry.tags.join(' ').toLowerCase().includes(query));
            let output = '';
            results.forEach(res => {
                output += `<p><b>Concept:</b> ${res.concept} <br><b>Rune:</b> ${res.rune} (Score: ${res.score}) <br><b>Excerpt:</b> ${res.excerpt}</p>`;
            });
            document.getElementById('results').innerHTML = output;
        }
    </script>
</head>
<body>
    <h1>The Aryanic Record</h1>
    <input id="query" type="text" placeholder="Search concepts or tags">
    <button onclick="searchDB()">Search</button>
    <div id="results"></div>
</body>
</html>
