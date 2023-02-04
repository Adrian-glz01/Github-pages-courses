# TAREA DE PRUEBA PARA EL CURSO "GITHUB-PAGES" DE GITHUB

**_CÓDIGO_**

```
public static boolean binarySearch(int[] numbers, int numberToSearch) {
    
  int size = numbers.length;  // Número de elementos
  int middle = size/2;        // Mitad del array
    
  System.out.println("Size: " + size);
  System.out.println("Middle: " + middle);
  System.out.println("Array: " + Arrays.toString(numbers));
    
  if (numbers[middle] == numberToSearch)
    return true;
  else if (size == 1)
    return false;
  else if (numbers[middle] > numberToSearch)
    return binarySearch(Arrays.copyOfRange(numbers,0,middle),numberToSearch);
  else
    return binarySearch(Arrays.copyOfRange(numbers,middle+1,size),numberToSearch);    
}

```
