package main

import "fmt"

func main() {
    testNums := []int{2, 7, 11, 15}
    target := 9
    result := twoSum(testNums, target)
    fmt.Println(result) // Output: [0 1]
}
func twoSum(nums []int, target int) []int {
    // map yaratamiz: key - sonning qiymati, value - uning indeksi
    m := make(map[int]int)

    for i, num := range nums {
        // Kerakli sonni hisoblaymiz
        complement := target - num

        // Map ichidan kerakli sonni qidiramiz
        if index, ok := m[complement]; ok {
            // Agar topilsa, o'sha sonning indeksi va hozirgi indeksni qaytaramiz
            return []int{index, i}
        }

        // Agar topilmasa, hozirgi sonni mapga saqlaymiz
        m[num] = i
    }

    // Hech narsa topilmasa bo'sh slice qaytaramiz
    return nil
}