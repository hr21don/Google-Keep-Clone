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
