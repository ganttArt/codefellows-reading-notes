# Forms

## [React Docs - Forms](https://reactjs.org/docs/forms.html)

- Forms in HTML already hold state, but in React we want to store state in one place, and that is in this.state.
- To do this, we write the form as a **Controlled Component**
- On submit we write a function to *handleSubmit*, *onChange*, and on the user inputing information the component uses a function, *handleChange*, to change *onchange* the state reactively as the user inputs information.

```javascript
class NameForm extends React.Component {
  constructor(props) {
    super(props);
    this.state = {value: ''};

    this.handleChange = this.handleChange.bind(this);
    this.handleSubmit = this.handleSubmit.bind(this);
  }

  handleChange(event) {
    this.setState({value: event.target.value});
  }

  handleSubmit(event) {
    alert('A name was submitted: ' + this.state.value);
    event.preventDefault();
  }

  render() {
    return (
      <form onSubmit={this.handleSubmit}>
        <label>
          Name:
          <input type="text" value={this.state.value} onChange={this.handleChange} />
        </label>
        <input type="submit" value="Submit" />
      </form>
    );
  }
}
```

- handleChange runs on every keystroke
- The docs continue by overviewing different tags and scenarios like, `<textarea> <select> <input type="file">`, handling multiple inputs, what to do with a null input value.
- Uncontrolled componenets is an alternate approach to dealing with forms.
- [Formik](https://jaredpalmer.com/formik) is a popular solution for working with forms in React.

## [React-Bootstrap Forms](https://react-bootstrap.github.io/components/forms/)

- Works similarly to other react-bootstrap tags. Use this in the JSX section of your component, but make sure to be including the handleChange and handleSubmit function references in the jsx for these form tags.
