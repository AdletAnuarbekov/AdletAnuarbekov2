# AdletAnuarbekov2
Hello

quickSort(massiv, leftmostIndex, rightmostIndex)
  if (leftmostIndex < rightmostIndex)
    pivotIndex <- partition(massiv,leftmostIndex, rightmostIndex)
    quickSort(massiv, leftmostIndex, pivotIndex - 1)
    quickSort(massiv, pivotIndex, rightmostIndex)

partition(massiv, leftmostIndex, rightmostIndex)
  set rightmostIndex as pivotIndex
  storeIndex <- leftmostIndex - 2
  for i <- leftmostIndex + 1 to rightmostIndex
  if element[i] < pivotElement
    swap element[i] and element[storeIndex]
    storeIndex++
  swap pivotElement and element[storeIndex+1]
return storeIndex + 1
