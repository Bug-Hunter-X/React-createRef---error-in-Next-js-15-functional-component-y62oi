# React.createRef() Error in Next.js 15 Functional Component

This repository demonstrates a subtle bug encountered in Next.js 15 when using `React.createRef()` within a functional component without the appropriate `useRef` hook.  The issue results in an error preventing the component from rendering correctly.

## Problem Description

Attempting to directly use `React.createRef()` in a functional component in Next.js 15 leads to an error because functional components require the `useRef` hook to manage references.

## Solution

The solution involves replacing the direct use of `React.createRef()` with the `useRef` hook. This ensures proper reference management within the functional component's lifecycle.