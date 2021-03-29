# CRUD

## [Sending Form Data](https://developer.mozilla.org/en-US/docs/Learn/Forms/Sending_and_retrieving_form_data)

- After a form is validated on the client-side, we can send it to our backend
- We'll send a request to a server using HTTP
- The action attribute defines where the data gets sent. Its value must be a valid relative or absolute URL. If this attribute isn't provided, the data will be sent to the URL of the page containing the form — the current page. `<form action="https://example.com">`
- The method attribute defines how data is sent
  - GET & POST
- Viewing HTTP Requests
  - Open the developer tools.
  - Select "Network"
  - Select "All"
  - Select "foo.com" in the "Name" tab
  - Select "Headers"
- Retrieve the data with a tool for the language you're using
  - Python: Flask or Django, Node: Express, Ruby: Ruby On Rails, Laravel: PHP
- Use enctype attribute to send file, include type="file" in input. `enctype="multipart/form-data">`
- Security:
  - Escape potentially dangerous characters
  - Limit the incoming amount of data to allow only what's necessary.
  - Sandbox uploaded files: Store them on a different server and allow access to the file only through a different subdomain or even better through a completely different domain.

How do I perform client-side form validation in Node or Express? express-validator is a potential option.
