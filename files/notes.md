# First Internship Notes

Summary of my highlights of my first internship.

## Mission of opus1.io

I will say that opu1.io mission is to provide, to business owners, a better
alternative of their management platform. Essentially, be able to grow their
business by automating a series of tasks, putting them like in autopilot,
so they and let it grow while focusing on what they love to do.

## Contributed Projects

During my time working as intern, I contributed to the following projects:

### opus1.io

![opus1io_logo](../Assets/logos/opus1io.png)

opus1.io is an ideal solution for personal services businesses,
small to large, especially for:

- Performing Arts Schools (Music, dance etc.)
- Kids activities (Tutoring, camps etc.)
- Wellness / Health businesses (Yoga, pilates, spas, salons etc.)
- Fitness, sports coaching & training
- Studios facilities & rental (Photography, recording etc.)

#### Main Features

What makes opus1.io special is:

- **Appointment scheduling**

Schedule your staff (instructors, teachers, coaches etc.) availabilities,
for specific services, locations and rooms and let your customers easily
self-book single or recurring appointments

- **Classes / Courses**

Schedule your classes sessions, capacity, enrollment windows, locations,
instructors, payment options and let your customer easily self-enroll and
access their schedule

- **Payment**

Take payment from your customers on a single or recurring basis, with
automated invoicing and competitively low credit card fees

- **Self-booking & Rescheduling**

Let your customers self-book and self-reschedule their appointments
with flexible policies that meet your business needs

- **Staff Management**

Manage your staff schedule, availabilities, pay rates, bonuses and
automate payroll

- **Clients / Families**

Manage your clients and families (e.g. mother, father, child, care taker).
You know who is taking the service, who is paying for it and
who to contact when needed

- **Automate Communications**

Automate communications with your clients (sign-up reminders,
appointment reminders, enrollment confirmation, cancellation policies,
payment reminders, invoices receipt etc.)

- **Optimize**

Visual your resources (locations, staff, rooms, equipment) utilization
and optimize to maximize your profit and growth

- **Analytics & Utilization**

Get a clear view of your business key metrics
(revenue, fill rate, membership, conversions)

### Axiad UnifiedUserPortal

![axiad_logo](../Assets/logos/axiad.png)

It's kinda a secret what I have done with an unnamed project from Axiad. ;)

...company info

## Results

During my internship period, I contributed to:

### Features

I made some cool feature, such as:

#### Hooks

< hook_definition />

- **useToggle**

I implemented to have a simple, yet common hook when
a toggling action is needed. I used it to be able
to toggle a modal.

- **useFetchData**

Because the app has about 42 restful api calls, we needed a way to reduce copy-paste code as much as possible. My boss guided me into creating this hook.

- **useSessionStorage**

This is another simple hook, but also very useful
when you need to save states (data) in a user session,
meaning that it will be persistent as long as he
doesn't logout or close the browser.

#### Components

< Component definition />

- **SearchBar**

Similar to AWS...

- **Modal Calendar**

A Modal ...

- **Operator Tab**

An example of a container-type component...

#### Styles and Design

...

- **Rebranding**

...

Screenshot of before and after...
Maybe blur if needed?

- **Theme**

By using `context`...

This is to be in accordance with the new company
image...

### Issues

...

#### Tests and Debugging

- **Unit**

Used `Jest` as the testing framework. Its focus is on simplicity. It Ensures that the tests have unique global state, making them run reliably in parallel.
It also runs previously failed tests first and re-organizes runs based on how long test files take. And did you know, it can also generate code coverage, collecting information from the entire project, including untested files.

- **End-to-end**

Used `selenium-webdriver` to create robust, browser-based regression automation suites and tests. Selenium is a browser automation library.

#### Refactoring

Major refactors that I made were:

- **Class Components to Functional Components**

React.js started like this...

```js
// Example of a variable function component
var MyComponent = React.createClass({
  getDefaultProps: function() {
    return {
      text: 'Hello World!'
    };
  },
  render: function() {
    return <h1>{this.props.text}</h1>;
  },
})
```

and then like this...

```js
// Example of a class component
class HelloWorld extends React.Component {
  constructor (props) {
    super(props);
  }
  render () {
    const { text } = props;
    return <h1>{text}</h1>
  }
}

HelloWorld.defaultProps = {
  text: 'Hello world!',
}
```

and now...

```js
// Example of a functional component
const HelloWorld = ({ text = 'Hello world!' }) => <h1>HelloWorld!</h1>
```

They are all equivalent!

- **Styled Components**

Used this module to unify styles between components.
It utilizes tagged template literals and the power of CSS, a, styled-components allows you to write actual CSS code to style your components. It also removes the mapping between components and styles. In other words... It. Is. Amazing.

#### Bug Fixes

I fixed some bugs, like:

- Fixed how scrollbars behave different between browsers... Hi Firefox!
- Calendar wasn't being render correctly because of
different browsers... Oh, hi again Firefox!
- Timezone related issues... Where is Firefox?

#### Setup and Cleanup

There was some setup and cleanup to be done.

- **Breaking Changes**

Had to make several updates to multiple packages. It  has been a while since the last round of updates, so
there where some breaking changes that we introduced.
I good example is `styled-components`, that changed the way to import a global style from one version to the other.

- **Scripts**

Made some scripts, like:

```
yarn debug-test   (jest-enviroment-node-debug)
yarn analyze     (source-map-explorer)
yarn test-report  (export test report to html)
```
- **Linter**

Used `eslint` as the linter to analyze the code to find problems that can be automatically fixed. It's similar to what we call in 42 "the norm". Our configuration is based on the AirBnB one, with some changes here and there...

- **Formatter**

Used `prettier` as the code formatter of our choice. It's an opinionated code formatter that supports many languages, and integrates easily with visual code. It's amazing because you press save and code is formatted, and there is no need to discuss style in code review.
