# 100 Days Of Code - Log

### Day 1: April 18, 2018

**Today's Progress**: Learning React.JS Part 1 - JSX Elements

**Thoughts:** I'm starting this challenge with learning React. My goal is to become a Front-End Developer, and to do so I need to pick up some JS Libraries like React and Node. I am going to be using Codecademy, which has been the most effective method of learning code for me.

**Image:** ![Learning JSX](https://raw.githubusercontent.com/sebastiandesign/100-days-of-code/master/images/screenshot1.png)

**Want to follow along?** https://www.codecademy.com/

### Day 2: April 19, 2018

**Today's Progress**: Learning React.JS Part 2 - Advanced JSX

**Thoughts:** There was a lot more information thrown at me, but I know that I'm not expected to remember it all at once. Even so, I'll recap so that I can look back and say, 'yeah, I remember that!'

**Lesson Recap:** 
- Use className instead of class for HTML elements. 
- Close img and br tags />. 
- Use curlys {} when injecting regular JS. 
- You can call variables with injected JS. 
- Write event listeners in camelCase. 
- Use if statements outside of JSX. 
- Remember x ? y : z (if x is true, execute y, else z). 
- Use .map() to make a list of JSX elements. 
- Use keys to order a list (key=" "). 
- You can write in React without JSX with React.createElement();.

**Image:** ![Advanced JSX](https://raw.githubusercontent.com/sebastiandesign/100-days-of-code/master/images/screenshot2.png)

### Day 3: April 20, 2018

**Today's Progress**: Learning React.JS Part 3 - React Components

**Thoughts:** I decided to challenge myself this time by trying to remember code from the previous two days. I can say I'm quite proud of myself. I can now make a component without having to look at the example code. Though I do have to admit it took me some time to create a conditional statement without using if/else. It wasn't required, but I wanted to try anyway.

**Image:** ![Components](https://raw.githubusercontent.com/sebastiandesign/100-days-of-code/master/images/screenshot3.png)

### Day 4: April 22, 2018

**Today's Progress**: Learning React.JS Part 4 - This.props & Event Handlers

**Thoughts:** I struggled for a while as I tried to understand what the Codecademy lesson was trying to tell me to do. I finally gave up and let it give me the answer, and I facepalmed. It's always that one small thing that messes you up...

**Lesson Recap:**
- Components can have properties (this.props)
- To render a prop:
```jsx
  render() {
    return <h1>Hello, {this.props.propName}</h1>;
  }
```
- To pass a prop:
```jsx
  ReactDOM.render(
    <className propName="Property"/>,
    document.getElementById('app')
  )
```
- Props are typically used to carry functions like event handlers
- Event handlers are defined like methods:
```jsx
   handleClick() {
    alert(`I am an event handler.
      If you see this message,
      then I have been called.`);
  }
```
- These event handlers are attached to events with ***this***:
```jsx
    <h1 onClick={this.handleClick}>
      Hello world
    </h1>
```
- The name of the event handler should be different from the event
- To pass the event handler as a prop from ***parent*** to ***child***:
```jsx
  render() {
    return <Button onClick={this.handleClick}/>;
  }
```
- To receive an event handler from ***parent***:
```jsx
  render() {
    return (
      <button onClick={this.props.onClick}>
        Click me!
      </button>
    );
  }
```

**Image:** ![Props](https://raw.githubusercontent.com/sebastiandesign/100-days-of-code/master/images/screenshot4.png)

### Day 5: April 24, 2018

**Today's Progress**: Learning React.JS Part 5 - This.state, Constructors and super(props)

**Thoughts:** Loved how there is no explanation as to why super(props) is needed in order to pass this to a state inside a constructor. Oh well, just another mystery to add next to how people still believe the world is flat.

**Lesson Recap:**
- Components can have states (this.state)
- Both props and states are known as dynamic information
- States are determined in the constructor method:
```jsx
  constructor(props) {
    //super(props) is needed to pass this to a state
    super(props);
    this.state = { mood: 'good' };
    //the event handler needs to be bound by this
    this.toggleMood = this.toggleMood.bind(this);
  }
```
- The event handler is in charge of changing the state:
```jsx
  toggleMood() {
    const newMood = this.state.mood == 'good' ? 'bad' : 'good';
    this.setState({ mood: newMood });
  }
```

**Image:** ![States](https://raw.githubusercontent.com/sebastiandesign/100-days-of-code/master/images/screenshot5.png)

### Day 6: April 25, 2018

**Today's Progress**: Learning React.JS Part 6 - Parent, Child and Sibling Components

**Thoughts:** It just gets more and more complicated. I think I should summarize each lesson so that all these concepts stick. For now, I'll go back and add a recap for this.props and this.state.

**Image:** ![Family of Components](https://raw.githubusercontent.com/sebastiandesign/100-days-of-code/master/images/screenshot6.png)

### Day 7: April 26, 2018

**Today's Progress**: Learning React.JS Part 7 - Advanced React Programming Patterns

**Thoughts:** I am 50% through the second part of Codecademy's React.JS course and I feel like I have a good grasp as to what is going on. I hope to make something useful from what I've learned soon.

**Image:** ![Advanced React](https://raw.githubusercontent.com/sebastiandesign/100-days-of-code/master/images/screenshot7.png)

### Day 8: April 28, 2018

**Today's Progress**: Learning React.JS Part 8 - PropTypes and React Forms

**Thoughts:** I'm deliberately trying to pace myself with this challenge. I don't want to invest so much that I end up burning out and dropping the ball. The thing is I'm constantly itching to code, so I need to force myself off the computer and find other things to do.

**Image:** ![React Forms](https://raw.githubusercontent.com/sebastiandesign/100-days-of-code/master/images/screenshot8.png)

### Day 9: April 29, 2018

**Today's Progress**: Learning React.JS Part 9 - Lifecycle Methods

**Thoughts:** One of the lessons took me through fixing a number target game, but even after having completed the lesson, it still wasn't a very functional game. Now that I'm done with my React lessons, I'm going to go back next time and make it work better as a challenge.

**Image:** ![Lifecycle Methods](https://raw.githubusercontent.com/sebastiandesign/100-days-of-code/master/images/screenshot9.png)

### Day 10: May 1, 2018

**Today's Progress**: Making a React.JS Game Part 1 - Number Target Game Fix

**Thoughts:** As per my last update, I went back and made a couple changes to the number target game to make it more functional. It worked! The problem now is that I want to show my work, but I'm not sure how to get a React app on GitHub. I guess that's my next challenge.

**Image:** N/A until I can figure the above out...
