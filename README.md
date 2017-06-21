# partial-json-parser
Parse complete javascript objects from partial JSON strings. Useful for parsing responses that are transferred using chunked transfer encoding. 

# Description
Incomplete JSON strings will be parsed to its nearest complete object. 

Input: 
`{
  name: {
    first: 'ind',
    last: 'go`
    
Output:
{
  name: {
    first: 'ind'
  }
}
