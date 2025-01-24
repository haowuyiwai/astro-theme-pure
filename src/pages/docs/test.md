---
layout: '@/layouts/DocsLayout.astro'

title: 'Shiki Code'
description: 'Some mmthods using shiki code'
---



test

test


## 标题


```java

public class BubbleSort {  
    public static void main(String[] args) {  
        int[] arr = {64, 34, 25, 12, 22, 11, 90};  
        bubbleSort(arr);  
        System.out.println("排序后的数组：");  
        printArray(arr);  
    }  

    // 冒泡排序方法  
    static void bubbleSort(int[] arr) {  
        int n = arr.length;  
        boolean swapped; // 用于检查每一轮是否发生了交换  
        for (int i = 0; i < n - 1; i++) {  
            swapped = false; // 每轮开始时设置为没有交换  
            
            for (int j = 0; j < n - 1 - i; j++) {  
                if (arr[j] > arr[j + 1]) {  
                    // 交换 arr[j] 和 arr[j+1]  
                    int temp = arr[j];  
                    arr[j] = arr[j + 1];  
                    arr[j + 1] = temp;  
                    swapped = true; // 发生了交换  
                }  
            }  
            // 如果没有发生交换，数组已经有序，提前结束  
            if (!swapped) break;  
        }  
    }  

    // 打印数组的方法  
    static void printArray(int[] arr) {  
        for (int num : arr) {  
            System.out.print(num + " ");  
        }  
        System.out.println();  
    }  
}
```