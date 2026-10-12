
# ESEP Grade Calculator

This is a simple grade calculator written in Go. It calculates a student's final letter grade based on assignments, exams, and essays.

## Requirements

- Go 1.24.4 or newer

## Project Files

- `go.mod` - Defines the Go module and version.
- `grade_calculator.go` - Contains the grade calculator code.
- `grade_calculator_test.go` - Contains unit tests.
- `README.MD` - Explains how to use the project.

## Grade Weights

- Assignments: 50%
- Exams: 35%
- Essays: 15%

The calculator finds the average of each category and uses these weights to calculate the final grade.

## Letter Grades

- A: 90-100
- B: 80-89
- C: 70-79
- D: 60-69
- F: Below 60

A grade of C or higher is passing.

## How to Run Tests

Open a terminal in the project folder and enter:

```bash
cd grade-calculator
go test -v ./...
```

## How to Check Code Coverage

Run:

```bash
go test -coverprofile=coverage.txt ./...
go tool cover -func=coverage.txt
```

## Example

```go
calculator := NewGradeCalculator()

calculator.AddGrade("Assignment 1", 90, Assignment)
calculator.AddGrade("Exam 1", 85, Exam)
calculator.AddGrade("Essay 1", 95, Essay)

finalGrade := calculator.GetFinalGrade()
```

The project currently has some issues in its code and tests that will be fixed in later steps.