# partial-json-parser
Parse complete javascript objects from partial JSON strings. I looked around a bit for something that could parse chunked data from a fetch request, but could not find an implementation that was either minimal or written in javascript. Tested this against some random nested data generated by www.json-generator.com, but there could still be issues if any string values contain escape characters.

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
