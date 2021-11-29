# Select Options Dump Demo

*Demonstrates a feature of adding options to a series of Select elements as well as removing any created element from all Selects.*

    const groupSelAll = getElementsbyClassName('groupSel');

is what is used to capture all of the Select Elements. So groupSelAll has it's own length, and each one of those selects has their OWN length AS WELL.

So when you go through the array of groupSelAll, you also have to go through the length of each one of those indexes. This is only necessary for removing options. When you add elements you simply append a new option element. review code below to see function for removing elements throughout entire select list

        function removeOptionFromAll(optionSel){
            for(let i = 0; i < groupSelAll.length; i++){
                for (let j = 0; j < groupSelAll[i].length; j++){
                    if (groupSelAll[i][j].textContent === optionSel){
                        groupSelAll[i][j].replaceWith();
                    }
                }
            }
        }
