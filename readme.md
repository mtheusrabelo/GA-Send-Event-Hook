# Google Analytics Send Event Hook

# Usage
The following code goes inside your component
```jsx
const Project = ({ url }) => {
  const sendEvent = useSendEvent();
  const event = {
      category: 'Project',
      action: 'click',
      label: url
  };

  return (
    <a href={url} target="_blank" rel="noreferrer" onClick={() => sendEvent(event)}>
      project
    </a>
  );
};
```

# License
MIT

# Author
Matheus Freire Rabelo
