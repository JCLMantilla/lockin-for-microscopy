# lockin-for-microscopy

Project summary: Digital Lock-in amplifier for signal multiplexing in microscopy
This is a digital implementation of a Lock-in amplifier, this assumes that every signal are in-phase with each other. We simulated noisy data collected by a CMOS camera from florescence signals emitted by a sinusoidal-illuminated 2D sample+. The nature of the noise is shot noise, or also known as Poisson noise.
A synthetic signal with a specific frequency was assigned to each row of pixels and then overlapped all together along the columns, collapsing one spatial component of the image. The Lock-in filtered every signal successfully form the noisy data, effectively retrieving the dimension lost due to the overlapping, and used to reconstruct the original image without losing too much information.
This project shows that a Lock-in amplifier is a good candidate to pre-process 3D images produced by digital micro-mirror devices (DMDs) in structured illumination microscopy.
