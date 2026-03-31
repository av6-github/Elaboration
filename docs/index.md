# Bag of Words

The codebase is designed to categorize/classify the columns present in the TSV input file into classes according to the existing categories present in the Neurobagel annotation tool, based on the column name and the content of the column. The LLM makes its predictions for a specific input string consisting of the column header and the column contents based on the examples provided to it beforehand in its prompt template. The various tasks carried out by this codebase mainly utilize LangChain, the json library from Python, and the LLM 'Gemma' from Ollama.



# Fuzzy Matching 
Fuzzy matching (or approximate string matching) is a data processing technique that identifies and links strings of text that are similar but not identical. Instead of requiring an exact character-by-character match, it uses algorithms to calculate a similarity score that accounts for typos, spelling variations, abbreviations, and formatting inconsistencies


#Zod Schema 

A Zod schema is an object defined using the Zod library that describes the expected structure and validation rules for a piece of data. It serves two primary purposes: providing runtime validation of data in JavaScript/TypeScript applications and automatically inferring static TypeScript types from a single source of truth. 

Key Concepts
-->  Runtime Validation: Unlike TypeScript's static type checks, which only happen during development (compile-time), a Zod schema validates data at runtime. This is crucial for data coming from external, untrusted sources like user form inputs, API responses, or configuration files, where the data is not guaranteed to match the expected structure.
--> Type Inference: Zod can automatically infer the static TypeScript type of the data structure from the schema using the z.infer<typeof yourSchema> utility. This prevents the need for writing duplicate type definitions and validation logic, ensuring type consistency throughout the application.
--> Composability: Zod schemas are highly composable. Simple schemas (like strings or numbers) can be combined to form complex, nested object and array schemas, which promotes code reuse and manageability in large applications
