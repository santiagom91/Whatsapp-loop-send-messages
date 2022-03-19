# Whatsapp-loop-send-messages
Whatsapp-loop-send-messages
The steps to send whatsapp messages on loop: 
1) Open Whatsapp web
2) Click on the person you want to send messages on loop
3) Open the browser console
4) Copy the code from below (*)
5) Paste the code in browser console.
6) Select enter then it will ask you to type your message and the number of times you want to send the message


(*)

```javascript
var message = prompt("Enter your loop message: ", "‎");
var counter = parseInt(prompt("How many times do you want to send the message?", 10));
window.InputEvent = window.Event || window.InputEvent;
var event = new InputEvent("input", { bubbles: true });
var textbox = document.getElementsByClassName("_13NKt copyable-text selectable-text")[1];
for (let index = 0; index < counter; index++) {
  textbox.innerHTML = message;
  textbox.dispatchEvent(event);
  document.getElementsByClassName("_4sWnG")[0].click();
}
```
