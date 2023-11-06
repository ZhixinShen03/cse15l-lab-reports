Part 1:
A failure-inducing input for the buggy program：
@Test
public void testFailureReverseInPlace() {
  int[] input = {1, 2, 3, 4};
  ArrayExamples.reverseInPlace(input);
  assertArrayEquals("Array with multiple elements should be reversed in place", 
                    new int[]{4, 3, 2, 1}, input);
}
