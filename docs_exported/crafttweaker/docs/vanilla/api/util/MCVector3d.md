# MCVector3d

A 3-dimensional vector, in a 3-dimensional vector space.

 This class is immutable, meaning its values cannot change, so it is safe to be stored as a key in maps or in
 collections.

 No, it's not an arrow.

## Importing the class

It might be required for you to import the package if you encounter any issues (like casting an Array), so better be safe than sorry and add the import at the very top of the file.
```zenscript
import crafttweaker.api.util.MCVector3d;
```


## Constructors


```zenscript
new MCVector3d(x as double, y as double, z as double) as MCVector3d
```

| Parameter | Type | Description |
|-----------|------|-------------|
| x | double | No description provided |
| y | double | No description provided |
| z | double | No description provided |



## Methods

:::group{name=cross}

Performs the cross product between this vector and <code>other</code>.

Return Type: [MCVector3d](/vanilla/api/util/MCVector3d)

```zenscript
MCVector3d.cross(other as MCVector3d) as MCVector3d
```

| Parameter | Type | Description |
|-----------|------|-------------|
| other | [MCVector3d](/vanilla/api/util/MCVector3d) | The other vector. |


:::

:::group{name=distanceTo}

Computes the Euclidean distance between this vector and the other vector.

Return Type: double

```zenscript
MCVector3d.distanceTo(other as MCVector3d) as double
```

| Parameter | Type | Description |
|-----------|------|-------------|
| other | [MCVector3d](/vanilla/api/util/MCVector3d) | The other vector. |


:::

:::group{name=dot}

Performs a dot product between this vector and <code>other</code>.

Return Type: double

```zenscript
MCVector3d.dot(other as MCVector3d) as double
```

| Parameter | Type | Description |
|-----------|------|-------------|
| other | [MCVector3d](/vanilla/api/util/MCVector3d) | The other vector. |


:::

:::group{name=getCoordinate}

Gets the coordinate of this vector that corresponds to the given [DirectionAxis](/vanilla/api/util/DirectionAxis).

Return Type: double

```zenscript
MCVector3d.getCoordinate(axis as DirectionAxis) as double
```

| Parameter | Type | Description |
|-----------|------|-------------|
| axis | [DirectionAxis](/vanilla/api/util/DirectionAxis) | The axis. |


:::

:::group{name=getCoordinate}

Gets the coordinate of this vector identified by the specified index.

 Namely, 0 corresponds to the X coordinate, 1 to Y, and 2 to Z.

Return Type: double

```zenscript
MCVector3d.getCoordinate(index as int) as double
```

| Parameter | Type | Description |
|-----------|------|-------------|
| index | int | The coordinate index. |


:::

:::group{name=minus}

Subtracts <code>other</code> from this vector.

Return Type: [MCVector3d](/vanilla/api/util/MCVector3d)

```zenscript
MCVector3d.minus(other as MCVector3d) as MCVector3d
```

| Parameter | Type | Description |
|-----------|------|-------------|
| other | [MCVector3d](/vanilla/api/util/MCVector3d) | The other vector. |


:::

:::group{name=minus}

Subtracts the vector <code>(x, y, z)</code> from this vector.

Return Type: [MCVector3d](/vanilla/api/util/MCVector3d)

```zenscript
MCVector3d.minus(x as double, y as double, z as double) as MCVector3d
```

| Parameter | Type | Description |
|-----------|------|-------------|
| x | double | The x component of the other vector. |
| y | double | The y component of the other vector. |
| z | double | The z component of the other vector. |


:::

:::group{name=normalize}

Normalizes the current vector, making it of unit length.

Return Type: [MCVector3d](/vanilla/api/util/MCVector3d)

```zenscript
// MCVector3d.normalize() as MCVector3d

myMCVector3d.normalize();
```

:::

:::group{name=plus}

Adds this vector to the <code>other</code> vector, computing their sum member by member.

Return Type: [MCVector3d](/vanilla/api/util/MCVector3d)

```zenscript
MCVector3d.plus(other as MCVector3d) as MCVector3d
```

| Parameter | Type | Description |
|-----------|------|-------------|
| other | [MCVector3d](/vanilla/api/util/MCVector3d) | The other vector. |


:::

:::group{name=plus}

Adds this vector to the vector <code>(x, y, z)</code>, computing their sum member by member.

Return Type: [MCVector3d](/vanilla/api/util/MCVector3d)

```zenscript
MCVector3d.plus(x as double, y as double, z as double) as MCVector3d
```

| Parameter | Type | Description |
|-----------|------|-------------|
| x | double | The x component of the other vector. |
| y | double | The y component of the other vector. |
| z | double | The z component of the other vector. |


:::

:::group{name=scale}

Scales the current vector by the given <code>factor</code>.

Return Type: [MCVector3d](/vanilla/api/util/MCVector3d)

```zenscript
MCVector3d.scale(factor as double) as MCVector3d
```

| Parameter | Type | Description |
|-----------|------|-------------|
| factor | double | The factor. |


:::

:::group{name=squareDistanceTo}

Computes the squared Euclidean distance between this vector and the other vector.

 This method is faster and less error-prone than calling <code>distanceTo</code> and squaring the result.

Return Type: double

```zenscript
MCVector3d.squareDistanceTo(other as MCVector3d) as double
```

| Parameter | Type | Description |
|-----------|------|-------------|
| other | [MCVector3d](/vanilla/api/util/MCVector3d) | The other vector. |


:::

:::group{name=subtractReverse}

Subtracts this vector from the <code>other</code> vector and returns the result.

Return Type: [MCVector3d](/vanilla/api/util/MCVector3d)

```zenscript
MCVector3d.subtractReverse(other as MCVector3d) as MCVector3d
```

| Parameter | Type | Description |
|-----------|------|-------------|
| other | [MCVector3d](/vanilla/api/util/MCVector3d) | The vector from which this vector should be subtracted from. |


:::

:::group{name=times}

Multiplies the two vectors member by member, computing what is known as the Hadamard product.

Return Type: [MCVector3d](/vanilla/api/util/MCVector3d)

```zenscript
MCVector3d.times(other as MCVector3d) as MCVector3d
```

| Parameter | Type | Description |
|-----------|------|-------------|
| other | [MCVector3d](/vanilla/api/util/MCVector3d) | The other vector. |


:::

:::group{name=times}

Multiplies this vector with the vector <code>(x, y, z)</code>, computing what is known as the Hadamard product.

Return Type: [MCVector3d](/vanilla/api/util/MCVector3d)

```zenscript
MCVector3d.times(x as double, y as double, z as double) as MCVector3d
```

| Parameter | Type | Description |
|-----------|------|-------------|
| x | double | The x component of the other vector. |
| y | double | The y component of the other vector. |
| z | double | The z component of the other vector. |


:::


## Properties

| Name | Type | Has Getter | Has Setter | Description |
|------|------|------------|------------|-------------|
| inverse | [MCVector3d](/vanilla/api/util/MCVector3d) | true | false | Inverts the vector, effectively flipping it. <br />  <br />  This is equivalent to a scale by -1, or a rotation of pi radians around the origin. |
| magnitude | double | true | false | Gets the length, also known as magnitude, of the vector. |
| magnitudeSquared | double | true | false | Gets the squared length, also known as squared magnitude, of the vector. <br />  <br />  This method is faster and less error-prone than calling <code>magnitude</code> and squaring the result. |
| x | double | true | false | Gets the X coordinate of this vector. |
| y | double | true | false | Gets the Y coordinate of this vector. |
| z | double | true | false | Gets the Z coordinate of this vector. |

