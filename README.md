def calculate_matrix_diagonal(matrix):
    return sum(
        matrix[index][index]
        for index in range(len(matrix))
    )


if __name__ == "__main__":
    matrix = [
        [5, 2, 1],
        [4, 8, 3],
        [7, 6, 9]
    ]

    print("Matrix:")
    for row in matrix:
        print(row)

    print(f"Main diagonal sum: {calculate_matrix_diagonal(matrix)}")
