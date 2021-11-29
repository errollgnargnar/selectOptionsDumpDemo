# select Options Dump Demo

Demonstrates a feature of adding options to a series of Select elements as well as removing any created element from all Selects.

    const groupSelAll = getElementsbyClassName('groupSel');

is what is used to capture all of the Select Elements. So groupSelAll has it's own length, and each one of those selects has their OWN length AS WELL.

So when you go through the array of groupSelAll, you also have to go through the length of each one of those indexes. 
