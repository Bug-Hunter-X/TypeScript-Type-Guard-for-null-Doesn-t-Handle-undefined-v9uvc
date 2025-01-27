# TypeScript Type Guard Issue: Handling undefined

This repository demonstrates a common issue encountered when using type guards in TypeScript.  Specifically, a type guard designed to handle `null` values may not correctly handle `undefined` values, potentially leading to runtime errors.

The `bug.ts` file contains the problematic code.  The `bugSolution.ts` file provides a corrected version that explicitly handles both `null` and `undefined`. 

## Problem

The initial code attempts to use a type guard to differentiate between null and non-null string values. However, it fails to account for `undefined` inputs resulting in a runtime error.