🔄 Geometric Transformations in 2D

1️⃣ Euclidean Transformations (Rigid Body Motion)
	•	Operations: Rotation + Translation
	•	Properties: Preserves shape and size (rigid).
	•	Matrix form:
x{\prime} = R \cdot x + t
where R = rotation matrix, t = translation vector.
	•	Demo: A square rotated and shifted.

⸻

2️⃣ Similarity Transformations
	•	Operations: Rotation + Translation + Uniform Scaling
	•	Properties: Preserves shape but not size.
	•	Special case: Affine transform with uniform scale factor k.
	•	Matrix form:
x{\prime} = kR \cdot x + t
	•	Demo: A square rotated, shifted, and scaled uniformly.

⸻

3️⃣ Affine Transformations
	•	Operations: Rotation, Translation, Scaling (uniform / non-uniform), Shear
	•	Properties: Preserves parallel lines, not angles/lengths.
	•	Matrix form (2×3):
\begin{bmatrix}
x{\prime} \\ y{\prime}
\end{bmatrix}

\begin{bmatrix}
a & b & t_x \\
c & d & t_y
\end{bmatrix}
\cdot
\begin{bmatrix}
x \\ y \\ 1
\end{bmatrix}
	•	Demo: A square warped into a rectangle/parallelogram.

⸻

4️⃣ Projective Transformations (Homography)
	•	Most general linear 2D warp
	•	Operations: Translation, Rotation, Scaling, Shear, Perspective warp
	•	Properties: Preserves straight lines, but parallel lines may meet at vanishing point.
	•	Matrix form (3×3):
x{\prime} \sim H \cdot x
where H is a 3×3 homography matrix in homogeneous coordinates.
	•	Demo: A square warped into a trapezoid (perspective view).

