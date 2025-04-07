# react-props

import React from "react";

function Member({ name, profession, Isemployee }) {
  return (
    <li>
      {Isemployee && (
        <div>
          {name}
          <br></br>
          {profession}
        </div>
      )}
    </li>
  );
}

export default function App() {
  return (
    <>
      <section>
        <h1>Secret members of society</h1>

        <ul>
          <Member name="Pratual" profession="SDK2" Isemployee={true} />

          <Member name="lodge" profession="intern" Isemployee={false} />
        </ul>
      </section>
    </>
  );
}
