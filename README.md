# React_NoteKeeperApp


## Example  App Code
```
import React from "react";
import Header from "./Header";
import Footer from "./Footer";
import Note from "./Note";
import Notes from "../notes";

function App() {
  return (
    // * => **
    <div>
      <Header />
      {Notes.map((single_note) => (
        <Note
          key={single_note.key}
          title={single_note.title}
          content={single_note.content}
        />
      ))}
      <Footer />
    </div>
  );
}
export default App;
```
## Example Footer Code
```
import React from "react";

function Footer() {
  const currentYear = new Date().getFullYear();
  return (
    <footer>
      <p> Copyright ⓒ {currentYear}</p>{" "}
    </footer>
  );
}

export default Footer;
```

## Example Header Code
```
import React from "react";

function Header() {
  return (
    <header>
      <h1>Keeper</h1>
    </header>
  );
}

export default Header;

```

## Example Note Code
```
import React from "react";

function Note(props) {
  return (
    <div className="note">
      <h1>{props.title}</h1>
      <p>{props.content}</p>
    </div>
  );
}

export default Note;

```

## Example Index.js Code
```
import React from "react";
import ReactDom from "react-dom";
import App from "./Components/App";

ReactDom.render(<App />, document.getElementById("root"));
```

## Example Note.js Code
```
const notes = [
  {
    key: 1,
    title: "Delegation",
    content:
      "Q. How many programmers does it take to change a light bulb? A. None – It’s a hardware problem"
  },
  {
    key: 2,
    title: "Loops",
    content:
      "How to keep a programmer in the shower forever. Show him the shampoo bottle instructions: Lather. Rinse. Repeat."
  },
  {
    key: 3,
    title: "Arrays",
    content:
      "Q. Why did the programmer quit his job? A. Because he didn't get arrays."
  },
  {
    key: 4,
    title: "Hardware vs. Software",
    content:
      "What's the difference between hardware and software? You can hit your hardware with a hammer, but you can only curse at your software."
  },
  {
    key: 5,
    title: "Big ideas pt 1",
    content: "Eat more sushi"
  },
  {
    key: 6,
    title: "Big ideas pt 2",
    content: "Eat more Fish"
  },
  {
    key: 7,
    title: "Big ideas pt 3",
    content: "Eat more Chicken"
  },
  {
    key: 8,
    title: "Big ideas pt 4",
    content: "Eat more Rice"
  },
  {
    key: 9,
    title: "Big ideas pt 5",
    content: "Eat more Salad"
  },
  {
    key: 10,
    title: "Big ideas pt 6",
    content: "Eat more Fruit"
  }
];

export default notes;

```

## Output

The example output can be found in the sandbox repo at https://1euro.csb.app/. 

<img width="827" alt="Capture" src="https://user-images.githubusercontent.com/91548582/143610109-11939d9d-3d3c-42f7-a82e-7a5397a18948.PNG">


