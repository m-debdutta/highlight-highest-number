delayedPrompt = (callback) => {
setTimeout(() => {
const input = prompt();
if(invalidInput){highlightHighestNumber()};
callback(input, element);
},delay);
}

main(){
  const number = [];
  delayedPrompt((input) => {
    addNumberToList();
    number.push(input)
    main();
  })
}

highlightHighestNumber(){
  element
}