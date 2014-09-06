UhhhYeah
This is a short text story game I'm working on. It can run as it is but I will be working on it to make it longewr and add more options.
========
var user = prompt("You walk into a house that has three doors. Which one will you enter, the first, second, or third?").toLowerCase();
switch(user) {
    case 'first':
        var firstBook = prompt("Inside the first door is a huge library filled with books. This place is full of ancient texts from a long time ago. Do you want to read a book?").toLowerCase();
        var firstExplore = prompt("Or would you rather explore?").toLowerCase();
        if(firstBook === 'yes' || firstExplore === 'yes') {
        console.log("Whatever you ended up doing, you managed to open up a secret passage! Going down the passage leads you to secret treasure! There are rubies and gold beyond your wildest dreams! Now, how to lug all this back to where you came from...");
        }
        else {
            console.log("You do nothing and just stand there until you hear a low growling behind you. Turning around you see a huge bear! You are no match for the animal and are devoured. Next time don't be so boring. The end.");
        }
        break;
    case 'second':
        var secondFood = prompt("Inside the second door is a grand dining hall. At once this was a great space filled with food and laughter, but now that joy has faded and left a decrepit, empty chamber in its place. You notice a buffet table with fresh food of all sorts sitting out. There sweet fruits, thirst quenching drinks, and delectable desserts laid out for anyone to help themselves. Will you take anytyhing?").toLowerCase();
        var secondSure = prompt("Are you sure? You are very hungry and thirsty and no one else is around to watch you take something.").toLowerCase();
        if(secondFood === 'no' && secondSure === 'yes') {
            console.log("You're smart enough to realise that something seems fishy about this situation. You high-tail it out of this building before anything else weird can happen.");
        }
        else {
            var eatFood = prompt("You decide to take something. Upon scanning the buffet table you see that you have three options. There is a large, cheesy pizza (the kind with stuffed crust!), a crystal pitcher full of tea, and a moist chocolate cake. Which one do you choose to eat?").toLowerCase();
            switch(eatFood) {
                case 'pizza':
                    console.log("You grab a slice of delicious, cheesy pizza. As you eat you notice that the cheese is becoming increasingly difficult to chew and swallow. As you take another bite and are trying to chew you realise that your mouth has been cemented shut by the cheese! You blunder around in a panic until you trip over a chair and hit your face on the hard ground. A warm feeling spreads over you as your vision blurs and goes black. You end up never getting back up. The end.");
                    break;
                case 'tea' :
                    console.log("As thirsty as you are, you excitedly gulp down the tea. After a few sips, however, your throat starts to burn. The burning grows and spreads thoughout your whole body. You cannot do anything to stop this sensation and eventually lose consiousness from the pain. Your vision fades to black. You have died. The end.");
                    break;
                case 'cake' :
                    console.log("You walk over to the cake and start eating as much as you can. You eat and eat cake, but you never seem to finish it. After eating so much you think you might burst, you turn to head out the door. However, you seem to have eaten so much you're too tired to move! You decide to sit down and take a nap. Too bad you never wake up from it. The end.");
                    break;
                default:
                console.log("You can't back out now! Please remember to either choose pizza, tea, or cake.");
            }
        }
        break;
    case 'third':
        var thirdCandle = prompt("Inside the third door is a huge master bedroom. This room was once warm and inviting, but now it is just cold and empty. After groping round in the dark you notice a small candle on a bedside table. Do you want to light the candle?").toLowerCase();
        var thirdMatches = prompt("Did you remember to bring some matches or a lighter?").toLowerCase();
        if(thirdCandle === 'yes' && thirdMatches === 'yes') {
            console.log("You light the candle. It emits a faint glow over the room. On the bed you can see an old piece of paper. Upon further exploration you realise the paper is depicting a treasure map! You leave the house to search for treasure immediately!");
        }
        else if(thirdCandle === 'no' && thirdMatches === 'yes') {
            console.log("Why did you bring the matches then? You continue to blunder around in the dark until you fall in a pit. Injured from your fall, you just lay there until you die. The end.");
        }
        else {
            console.log("Standing in a dark, abandoned room fo so long gives you chills, so you decide to leave. As you head back the way you came, you bump into a huge, dark figure. The figure grabs you by your arms and throws you to the ground. Injured, you are not able to fight back as the figure slowly chokes you to death. The end.");
        }
        break;
    default:
        console.log("I can't understand that command. Please type either first, second, or third.");
}
