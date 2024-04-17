Assignment 05 - Sorting Algorithms
----------------------------------


The countingSort.html file includes an example of this algorithm implemented in JavaScript


In the sortingAlgorithm.html file, implement your assigned algorithm using JavaScript. 




- List your original group members: Dina, Julius, and Noah


- List anyone you worked with on the programming part: Dina, Julius, and Noah


- List any sites / videos /  chat GPT prompts you used to implement your code:
Chat GPT Prompt: using a bucket sort algorithm, sort a random list of 10 numbers from smallest to largest using javascript
https://medium.com/karuna-sehgal/an-introduction-to-bucket-sort-62aa5325d124


- Psuedocode for bucket sort implemented:
Find the minimum and maximum values in the input array
    min = inputArr[0]
    max = inputArr[0]
    for each element in inputArr, starting from the second element:
        if element < min, set min = element
        if element > max, set max = element

Create buckets based on the range of values
    Define bucketSize = 10
    Calculate the number of buckets required:
        bucketCount = (max - min) / bucketSize + 1
    Create an array of empty buckets:
        buckets[bucketCount]

Distribute elements into buckets
    for each element in inputArr:
        Calculate the index of the bucket where the element belongs:
            bucketIndex = (element - min) / bucketSize
        Add the element to the corresponding bucket:
            buckets[bucketIndex].push(element)

Sort each bucket individually
    for each bucket in buckets:
        Sort the elements in the bucket in ascending order

Concatenate the sorted buckets to form the sorted array
    Initialize an empty array to hold the sorted output:
        outputArr
    for each bucket in buckets:
        Append the elements of the bucket to the output array:
            outputArr.push(...bucket)

Return the sorted array
    return outputArr
