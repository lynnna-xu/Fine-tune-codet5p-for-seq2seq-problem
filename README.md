# Fine-tune-codet5p-for-seq2seq-problem
This notebook is dedicated to the fine-tuning of Large Language Model (LLM) to address a sequence-to-sequence problem. Our goal is to develop a versatile tool capable of translating user queries into API calls.

The tool's primary function is to interpret user queries and perform one of three types of operations:

Unit Conversion: It can convert units from one measurement to another. For example, from feet to centimeters, or kilograms to ounces.

Math Calculations: It can handle various mathematical calculations, including basic arithmetic (e.g., addition and subtraction) and more advanced operations (e.g., logarithm).

Search Queries: For general queries, it acts as a search engine, looking up information with no parameters.

Examples shown as below:

Input: “ft to cm”; output: “UnitConvert(SourceUnit:foot, TargetUnit:centimeter,

SourceValue:1)”

Input: “how many ounces in 5.8 kilograms”; output: “UnitConvert(SourceUnit:kilogram,

TargetUnit:ounce, SourceValue:5.8)”

Input: “two to the power of 10”, output: “Calculate(2^10)”

Input: “2001-1989”, output: “Calculate(2001-1989)”

Input: “what is chatgpt”, output: “Search()”

Input: “primary year 1 maths calculation checklist”, output: “Search()”

Input: “what are different length units”, output: “Search()”
