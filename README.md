# Hello there
Here you can get your own template to make a bingo game !

To do so all you need to do is go to [Releases](https://github.com/ENEexe/bingo-master) page and get the latest HTML file.

# How to modify your bingo board

Once you got the master file you will need to open it with any IDE or text editor. 
- (I suggest Notepad++ or Visual Studio Code, easy to use and they are free)

You will find all the needed information to make you custom bingo board inside.

And if that's a bit confusing to you there's a step-by-step guide below.

# How to make your own bingo board

## 1. Add you prompts to the collection !
- You will find a variable named `collection`, to add your prompt simply paste your text inside the square brackets.
- Example `const collection = ["Example item 1", "Example item 2", "Example item 3"]`
- In the example above, collection consists of 3 items.
- Note that items must be wrapped in quotation marks and separated by a comma.



## 2. Add your title !
- Pretty straightforward, you will find a line of code responsible for title at the top, change the text inside to your desired title.
- If you want to add any subtitle you can just copy the title line of code and paste it below.



## 3. Modify the grid dimensions !
- By default the grid is set to 5x5.
- If you want to add more to the grid you will need to add more rows and cells.
- You will find these lines of code:
```
<tr id="GRID-ROW">
     <td class="cell" id="GRID-CELL"></td>
     <td class="cell" id="GRID-CELL"></td>
     <td class="cell" id="GRID-CELL"></td>
     <td class="cell" id="GRID-CELL"></td>
     <td class="cell" id="GRID-CELL"></td>
</tr>
```
- Each such block is responsible for a single row of cells.
- To add more rows simply copypaste the block.
- And to add more cells you will need to add this `<td class="cell" id="GRID-CELL"></td>` inside the GRID-ROW element.
- Example row that has 9 cells will look like this:
```
<tr id="GRID-ROW">
     <td class="cell" id="GRID-CELL"></td>
     <td class="cell" id="GRID-CELL"></td>
     <td class="cell" id="GRID-CELL"></td>
     <td class="cell" id="GRID-CELL"></td>
     <td class="cell" id="GRID-CELL"></td>
     <td class="cell" id="GRID-CELL"></td>
     <td class="cell" id="GRID-CELL"></td>
     <td class="cell" id="GRID-CELL"></td>
     <td class="cell" id="GRID-CELL"></td>
</tr>
```
- Note that in order for a board to look good the grid dimensions should be odd numbers (i.e. 3x3, 5x5, 7x7, 9x9, etc.)
- Also don't forget to add the cells to the middle row

  

## 4. Modify the number of prompts generated for the board !
- You will find this line `const randomValues = getRandomValues(collection, 25)` below the collection.
- The number inside must be equal to the total number of cells
- So for 5x5 grid it's 25, for 7x7 it will be 49, and so on.

  

## 5. There is a promo section !
- If you want to add any promo, you can do so by editing a line of code in the promo section.
- There are comments inside that will help you to figure out how to make your links.
- If you don't need this section - just comment out or delete the code inside (to comment out a line of code you can highlight the desired lines and use `CTRL + /`)


## 6. There is also a Konami Code secret !
- You will find a section responsible for Konami code secret.
- There are three things in total you will need to modify there.
- They are highlighted with a commented text.
- If you don't want this in your bingo - simply delete the section or comment it out with `CTRL + /`

## 7. You are all set to publish your bingo ! 
- PLEASE use this [GUIDE](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site) as a reference.
- To publish your page you will first ned to create your own repository on GitHub.
- Rename the file you just made to  `index.html` and add it to your new repository.

# Have more questions ? 
You can contact me on discord DMs @ `ene.senkou`
