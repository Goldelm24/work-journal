## Learning about routing & navigation in Nextjs

A Dynamic segment can be created by wrapping a folder's name in square brackets:
`[folderName]`. Example: `[id]` or `[slug]` <br/>
### Dynamic routes <br/>
is a route with a parameter. Below is an example of how it works using Typescript. One of the beauties of working with `Typescript` is that it makes it easier to catch and prevent certain types of bugs which helps improve code quality. 

```
interface Props {
    params: { id: number; photoId: number}
}

const PhotoDetail = ({ params: {id, photoId}}: Props) => {
  return (
    <div>
      Photo{id} {photoId}
    </div>
  )
}

export default PhotoDetail;
```
### Catch-all Segments
Dynamic segments can be extended to catch-all susbsequent segments by adding an ellipsis inside the brackets. <br/>
Example: `pages/products/[[...slug]]`
