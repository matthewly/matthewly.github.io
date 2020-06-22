---
layout: post
title: Fetch data externally from API in ReactJS
---

*Have you ever tried creating a ReactJS application and wondered how to import data that is managed by an external service? Well I have, and here I will show you an example of how it is done.*


The job of ReactJS is to render UI components based on props and state. To get external data into your web app, you can perform these steps:

1. **Fetch data from the external service.** We can use the _axios_ http library to make the request to the external API. Note that we chain the request with a `.then( ... )` to parse the response.
```javascript
const url = /* API endpoint here */;
axios.get(url).then(res => {
    /* parse response here */
});
```

2. **Store it into the component's state.** We can do this by parsing the API response and setting the component's state.
```javascript
const users = res.data.results;
this.setState({ users });
```

3. **Re-render component after it is added to the DOM.** We can achieve this by adding steps 1 & 2 into the _componentDidMount_ lifecycle method.
```javascript
componentDidMount() {
    /* code from steps 1 & 2 here*/
}
```

See my example here:
[https://codesandbox.io/s/loving-shtern-fln8d](https://codesandbox.io/s/loving-shtern-fln8d)

