# Single Page Applications with Vue
01. What is the entrypoint of an application?

  > | Main.js is the entry point to an application and where the app is created. |

02. What is the difference between a vue `component` and `page`?

  > | Components are reusable code that can be used individually within pages. Pages are a view that components are used in pages work within router view. |

03. What is ***Component-Based Architecture***?

  > | Used for encapsulating individual pieces from a ui and being able to reuse that in different parts of ui. |

04. What are the three tags that make up a Vue component?

  > | Template, Script, Style |

05. What are ***lifecycle hooks***? What are lifecycle hooks used for?

  > | Lifecycle hooks allow you to know when your component is created, added to the DOM, updated, or destroyed. Used to mount and unmount components for better optimization for the application to be able to tell if the component needs to be running or not to save memory and avoid memory leaks. |

06. Which component in Vue does the vue-router use to mount pages onto?

  > | router-view |

07. What is the difference between the `AppState` and the state object within a component?

  > | The appstate is global within application and the state is like a local appstate within that specific component only. |

08. What is the responsibility of `Services` in our Vue projects?

  > | to change data within the appstate. |

09. What are ***props*** and how are they used? Provide an example

  > | props are used to pass variables and other info between components  |

10. What is the Vue method used to create watchable objects such as `state` or `AppState`?

  > | vue.observable or reactive or ref |
