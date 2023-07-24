# to-ini.py

A script to a file into an ini file.
Supports:
- JSON
- YAML

## Dependencies

Install dependencies by running:
`pip install -r requirements.txt`

## Usage
`to-ini [-h] -f FILE [-s SECTION]`

JSON:
		- If the value is a nested object the key for the object will become the section header, and the contents of the nested object will be as key-value pairs under the section.
	- If the value is a non-object/non-array type, the INI will reflect it as a key-value pair (including at top level).
	- If the value is an array the key for the array will become the section header
			each item will be given a key of the array's key (Ex. key-0 ... key-n)

## Contributing

Pull requests are welcome. For major changes, please open an issue first
to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License

[MIT](https://choosealicense.com/licenses/mit/)
