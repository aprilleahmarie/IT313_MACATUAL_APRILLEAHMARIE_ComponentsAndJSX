# IT313 - Components and JSX

## Student Roster Card Renderer

This project is a React Native Expo application that displays a list of students using reusable components.

## Problem

The application displays each student using a student card. Each card shows the student's name, course, and units enrolled. A "Full Load" label appears only when the student's `isFullLoad` value is true.

The application also displays the total number of students dynamically.

## Component Structure

### StudentCard

`StudentCard` is a functional component that receives:

- name
- course
- units
- isFullLoad

It uses props destructuring and JSX to display the student's information. Conditional rendering with `&&` is used for the "Full Load" label.

### StudentRoster

`StudentRoster` is the parent component that contains the students array.

It uses `.map()` to render one `StudentCard` for each student. Each card uses the student's unique ID as its key.

```jsx
key={student.id}