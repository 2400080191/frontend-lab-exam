import React, { useState } from "react";

function Counter() {
  const [count, setCount] = useState(0); // state to store counter value

  return (
    <div style={{ textAlign: "center", marginTop: "50px" }}>
      <h2>Counter Value: {count}</h2>

      <button
        style={{
          margin: "8px",
          padding: "10px 20px",
          backgroundColor: "green",
          color: "white",
          border: "none",
          borderRadius: "8px",
          cursor: "pointer",
        }}
        onClick={() => setCount(count + 1)}
      >
        Increment
      </button>

      <button
        style={{
          margin: "8px",
          padding: "10px 20px",
          backgroundColor: "red",
          color: "white",
          border: "none",
          borderRadius: "8px",
          cursor: "pointer",
        }}
        onClick={() => setCount(count - 1)}
      >
        Decrement
      </button>

      <button
        style={{
          margin: "8px",
          padding: "10px 20px",
          backgroundColor: "blue",
          color: "white",
          border: "none",
          borderRadius: "8px",
          cursor: "pointer",
        }}
        onClick={() => setCount(0)}
      >
        Reset
      </button>
    </div>
  );
}

export default Counter;
