# **Lab Report 3**
---
## Part 1 - Bugs
*Faulty Test*
```
 @Test
  public void testReverseInPlace2(){
    int[] input1 = { 3, 4, 5, 6};
    ArrayExamples.reverseInPlace(input1);
    assertArrayEquals(new int[]{6, 5, 4 , 3}, input1);
  }
```

*Passing Test*
```
@Test 
	public void testReverseInPlace() {
    int[] input1 = { 3 };
    ArrayExamples.reverseInPlace(input1);
    assertArrayEquals(new int[]{ 3 }, input1);
	}
```

*Output of both tests*



![Code Image](Lab-report-3-output.png)


*Buggy Code*
```
static void reverseInPlace(int[] arr) {
    for(int i = 0; i < arr.length; i += 1) {

      arr[i] = arr[arr.length - i - 1];

    }
  }
```

*Correct Code*
```
 static void reverseInPlace(int[] arr) {
    for(int i = 0; i < arr.length/2; i += 1) {
      int temp = arr[i];
      arr[i] = arr[arr.length - i - 1];
      arr[arr.length - i - 1] = temp;
    }
  }
```

Changing the function actually switches the values on both halfs of the array. before hand, it was just swapping positions regardless and would mess up the output that we desired. By only looping through the first half, we make sure we are not swapping the position of values twice therefore confirming they are in the correct position.
