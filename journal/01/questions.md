# Foundations of Web Development

1. In your own words, why do we use Git?

   > | Git and its version control as well as keeping our projects in order is incredibly important. It is a control system used to handle small to very large projects efficiently. Git is used to track changes in the source code, enabling multiple developers to work together on non-linear development. |

2. In the terminal, what is the command `mkdir` used for?

   > | mkdir is used to create a new directory in the current pathway |

3. What is a **_pseudo-class_** and what are some of the most common ones you think you will use?

   > | A pseudo-class is used to define special states of an element. For ex/ button:hover will allow us to affect the styles of the button when the mouse hovers over it. I think i'll end up using ':hover' a lot but there are many others, including pseudo elements (::) that I'll use too |

4. What is **_specificity_** and how might you use it to your benefit?

   > | Specificity is the algorithm used by browsers to determine the CSS declaration that is the most relevant to an element, which in turn, determines the property value to apply to the element. This includes ID selectors, CLASS selectors and TYPE selectors (ex/ p, h1, and td, and pseudo-elements like ::before). These are incredibly important and benefit me since they'll allow me to add specific and unique styles to whatever I add and add a certain value to them that overwrites the importance of other selectors, etc. |

5. What problems do you think you could run into if you over-utilized the `!important` feature?

   > | The !important rule has a higher importance value and will override ALL previous styling rules for the specific property on an element. This can lead to unintended consequences and make your code difficult to maintain and debug |

6. What are the three components that makeup a `CSS` rule? <br> Example:

   ```css
   h1 {
   	color: rgba(255, 210, 33, 0.75);
   }
   ```

   > | CSS's 3 components are the selector, property, and value. Selector (h1) names the rule and/or identifies its type. Property (color) is the style element being defined. Value (255, 210, 33, 0.75) is, of course, the value being assigned to the property. |

7. How do you think good design influences people when visiting a website, and what sorts of things could you convey through design alone?

   > | Good design influences a lot, if not, most things. Good design dictates wether the user continues and/or enjoys using the site. Things such as visuals that make the site look good to the eye, keep the user engaged. Good functionality design determines wether the users get frustrated using the site or even continue using the site at all. Good layout design can make things easier or harder to find for the users and how long it takes them to complete their task. Many things play into good design, specifically things making the experience as easy/comfortable as possible for the user. Things that can be conveyed include association (blue for medical, warm colors for food related things, etc), feelings of the designer (coding can be a lot like art; its expressive), and many many other things. |

8. What is the purpose of **_wireframing_**?

   > | A wireframe is commonly used to layout content and functionality on a page which takes into account user needs and user journeys. Wireframes are used early in the development process to establish the basic structure of a page before visual design and content is added. Wireframes serve multiple purposes by helping to: Connect the site's information architecture to its visual design by showing paths between pages. Clarify consistent ways for displaying particular types of information on the user interface. Determine intended functionality in the interface. |

9. Do you think wireframes are worth the time, energy, and effort that they require? Why or Why not?

   > | While creating a complex wireframe might take some time, it's definitely worth it. With it, you can get the client to review and accept key mechanics and elements of website structure. Wireframes are unique in that they help you get to a design solution quickly and make it easy to communicate the solution to different kinds of people. Unlike other design techniques, they support both divergent and convergent processes equally well. Divergence is the process of exploring and generating a wide range of ideas and possibilities without any judgment or criticism. Convergent thinking refers to the process of selecting, evaluating, and refining the most promising ideas from the divergent phase.|

10.   Define the display `:flex property:`

      > | The display: flex property sets your container to be a flexbox element. Enabling the flexbox layout mode lets you manipulate elements' alignment, spacing, and order within a container. .class {display: flex;} |

11.   What `CSS` properties affect the size of a box model?
      > | The CSS box model is a container that contains multiple properties including borders, margin, padding, and the content itself. In the standard box model, if you set inline-size and block-size (or width and height) property values on a box, these values define the inline-size and block-size (width and height in horizontal languages) of the content box. You can also just list the width, height, padding, border, and margin properties by themselves with their values to change the size of the box model. |
