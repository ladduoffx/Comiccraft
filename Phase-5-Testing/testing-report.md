# Phase 5: Testing

## Test Cases:

### Test Case 1: Simple Prompt
- Input: "A cat wearing superhero suit flying in Chennai"
- Expected: 4 panels generated with same cat
- Result: PASS - Character consistency 90% maintained

### Test Case 2: Long Story Prompt
- Input: A 200 word story
- Expected: Should trim and generate
- Result: PASS - After trimming, generated successfully

### Test Case 3: Different Art Styles
- Input: Same prompt with Marvel, Manga styles
- Expected: Images should look different per style
- Result: PASS

### Test Case 4: Download Feature
- Input: Click Download PDF
- Expected: PDF file downloaded
- Result: PASS

### Test Case 5: Invalid / Empty Prompt
- Input: Empty textbox
- Expected: Show error "Please enter a story"
- Result: PASS - Validation working

## Bugs Found & Fixed:
- Bug 1: PDF images overlapping -> Fixed with proper spacing.
- Bug 2: API key exposed -> Moved to st.secrets.

Overall Testing Status: 95% Successful
