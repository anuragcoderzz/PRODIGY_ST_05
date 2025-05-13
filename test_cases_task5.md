# Test Cases for Automation Practice Search Functionality

## Overview
These test cases are created for the Automation Practice e-commerce website (http://www.automationpractice.pl/index.php) to verify its search functionality. The test cases cover scenarios such as valid search, invalid search, partial match, and case sensitivity.

## Test Case 1: Valid Search with Correct Product Name
- **Test Case ID**: TC_01  
- **Test Description**: Verify that the search functionality returns correct results for a valid product name.  
- **Preconditions**: User is on the Automation Practice homepage (http://www.automationpractice.pl/index.php).  
- **Test Steps**:  
  1. Locate the search bar at the top of the page.  
  2. Enter "Dress" in the search bar.  
  3. Click the search button (magnifying glass icon).  
- **Expected Results**: Search results page is displayed, showing products related to "Dress" (e.g., "Printed Dress", "Evening Dress").

## Test Case 2: Invalid Search with Non-Existent Product
- **Test Case ID**: TC_02  
- **Test Description**: Verify that the search functionality handles a non-existent product name appropriately.  
- **Preconditions**: User is on the Automation Practice homepage.  
- **Test Steps**:  
  1. Locate the search bar at the top of the page.  
  2. Enter "xyz123" in the search bar.  
  3. Click the search button.  
- **Expected Results**: Search results page displays a message: "No results were found for your search 'xyz123'".

## Test Case 3: Partial Match Search
- **Test Case ID**: TC_03  
- **Test Description**: Verify that the search functionality returns results for a partial product name.  
- **Preconditions**: User is on the Automation Practice homepage.  
- **Test Steps**:  
  1. Locate the search bar at the top of the page.  
  2. Enter "Dres" in the search bar (partial match for "Dress").  
  3. Click the search button.  
- **Expected Results**: Search results page is displayed, showing products related to "Dress" (e.g., "Printed Dress", "Evening Dress").

## Test Case 4: Case Sensitivity in Search
- **Test Case ID**: TC_04  
- **Test Description**: Verify that the search functionality is not case-sensitive.  
- **Preconditions**: User is on the Automation Practice homepage.  
- **Test Steps**:  
  1. Locate the search bar at the top of the page.  
  2. Enter "dress" (lowercase) in the search bar.  
  3. Click the search button.  
  4. Clear the search bar and enter "DRESS" (uppercase).  
  5. Click the search button again.  
- **Expected Results**: Both searches ("dress" and "DRESS") return the same results, showing products related to "Dress".

## Test Case 5: Empty Search Query
- **Test Case ID**: TC_05  
- **Test Description**: Verify that the search functionality handles an empty search query appropriately.  
- **Preconditions**: User is on the Automation Practice homepage.  
- **Test Steps**:  
  1. Locate the search bar at the top of the page.  
  2. Leave the search bar empty.  
  3. Click the search button.  
- **Expected Results**: Search results page displays a message: "Please enter a search keyword".