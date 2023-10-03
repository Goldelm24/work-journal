## Learning about routing & navigation in Nextjs

Dynamic routes is a route with a parameter. Below is an example of how it works 

```interface Props {
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

