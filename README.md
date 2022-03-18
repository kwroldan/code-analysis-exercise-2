# Programming Exercise

Your task is to figure out how this code works.

* Come with a test input for the function.
* Trace the flow of the program with your test input **without running the code**, keeping track of all of the variables and transformations until you can determine the output.
* Keep coming up with new inputs until you're confident until you're confident that you know how the function works.
* Write a summary of what the function does.

**SUMMARY** 
The function tells you how many floors you are away from the ground floor. Buildings do not have 13th floors; therefore, whenever you are on a floor greater than or equal to 13, you are actually on the 14th or higher floor. 

```js
function (floor){
  if (floor <= 0){
    return floor
  }

  let offset = 1
  if (floor >= 13){
    offset = 2
  }

  return floor - offset
}
```

| Input | Output |
| ----- | ------ |
|    2  |    1   | 
|   14  |   12   | 
|    8  |    7   | 

<table>
  <tr>
    <th>What does this program do?</th>
    <td>The program takes your input, determines: 1) if the number is less than or equal to 0, if not then 2) checks if the number is greater than or equal to 13, and then finally 3) takes your input and subtracts an offset from it (depending on if your input met one of the parameters laid out in 1) or 2)). </td>
  </tr>
</table>

## Rubric

* Contains a plausible collection of test cases
* Outputs are accurately derived from inputs
* Summary is plausible
