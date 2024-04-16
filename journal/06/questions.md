# Single Page Applications with Vue
01. What is the entrypoint of an application?

  > | An application entry point identifies a resource that is an access point to an application. Application entry points are used to control users' access to different versions of an application that is deployed on a platform. |

02. What is the difference between a vue `component` and `page`?

  > | A component defines a part of a page. It can contain layout information, for example, content fields and placeholders, and their positions on the page, as well as business logic or metadata for the page. Typically, you reuse components on multiple pages. |

03. What is ***Component-Based Architecture***?

  > | Component-based architecture is a framework for building software based on reusable parts. Each component contains well-defined functionality into a binary unit that is stored in a library and then dropped into an application without modifying other components. The benefits include reduced development and testing time, enhanced reliability (because components are pre-tested), and the flexibility to change applications by adding or replacing components without significant disruption. |

04. What are the three tags that make up a Vue component?

  > | <script> <template> <style> |

05. What are ***lifecycle hooks***? What are lifecycle hooks used for?

  > | Your application can use lifecycle hook methods to tap into key events in the lifecycle of a component or directive to initialize new instances, initiate change detection when needed, respond to updates during change detection, and clean up before deletion of instances.  |

06. Which component in Vue does the vue-router use to mount pages onto?

  > | The RouterView component tells Vue Router where to render the current route component. That's the component that corresponds to the current URL path. It doesn't have to be in App.vue, you can put it anywhere to adapt it to your layout, but it does need to be included somewhere, otherwise Vue Router won't render anything. |

07. What is the difference between the `AppState` and the state object within a component?

  > | ANSWER HERE |

08. What is the responsibility of `Services` in our Vue projects?

  > | Services are focused pieces of reusable and testable code that you can use across your application. Thinking of any logic in your application as a collection of services can help you structure everything in a more maintainable way. The service should handle most of the logic, leaving controllers to do as little heavy lifting as possible( In Vue scenario: Let Vue handle synchronization between DOM and javascript, rest can be done in service). |

09. What are ***props*** and how are they used? Provide an example

  > | Props is a keyword that stands for Properties. Props are how we pass variables and other information around between different components. This is similar to how in Javascript we can pass variables into functions as arguments. |
	> | -----------------------------------------------
	> | <template>
	> |	<Camera 
	> |		name="Sony A7RIV" 
	> |		img="../sony-a7riv.jpg" 
	> |	/>
	> | </template> |
	> | -----------------------------------------------
	> | <template>
	> | 	<div class="camera">
	> | 		<h2 class="camera__name"></h2>
	> | 		<img class="camera__image" src="img" />
	> | 	</div>
	> | </template> |
	> | -----------------------------------------------
	> | <template>
	> | 	<Camera
	> | 		v-bind:name="cameraName"
	> | 		v-bind:img="cameraImage"
	> | 	/>
	> | </template>
	> | ----------------------------------------------- OR
	> | <template>
	> | 	<Camera
	> |		:name="cameraName"
	> |		:img="cameraImage || '../no-camera-found.jpg'"
	> | 	/>
	> | </template>
	> | -----------------------------------------------
	> | export default {
	> | 	name: 'Camera',
	> | 	props: {
	> | 		name: {
	> | 			type: String,
	> | 		},
	> |		img: {
	> | 			type: String,
	> |		}
	> |	}
	> | }



10. What is the Vue method used to create watchable objects such as `state` or `AppState`?

  > | With Composition API, we can use the watch function to trigger a callback whenever a piece of reactive state changes. There are multiple types of watchers as well. These include deep watchers, eager watchers, and once watchers. It is common for the watcher callback to use exactly the same reactive state as the source in which you would use watchEffect(). WatchEffect() allows us to track the callback's reactive dependencies automatically. |
