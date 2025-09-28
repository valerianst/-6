//TIP To <b>Run</b> code, press <shortcut actionId="Run"/> or
// click the <icon src="AllIcons.Actions.Execute"/> icon in the gutter.
fun frequencySort(arr: IntArray): IntArray {
    // Счет частоты каждого элемента
    val frequencyN = mutableMapOf<Int, Int>()
    for (num in arr) {
        frequencyN[num] = frequencyN.getOrDefault(num, 0) + 1
    }

    // Сортировка по частоте (убывание), а при равной частоте - по значению (возрастание)
    return arr.sortedWith(compareByDescending<Int> { frequencyN[it] }
        .thenBy { it })
        .toIntArray()
}

fun main() {
    val input = intArrayOf(4, 5, 6, 5, 4, 3)
    val result = frequencySort(input)

    println("Вход: ${input.joinToString()}")
    println("Выход: ${result.joinToString()}")
}

