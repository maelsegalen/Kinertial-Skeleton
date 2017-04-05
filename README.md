# Kinertial-Skeleton
Patch Max fusionnant les données de capteurs inertiels et d'exo-squelette kinect.


Ce patch Max est destiné à pallier aux problèmes de superposition des bras de la kinect (et donc aux pertes de tracking).

Le patch positionne la personne dans l'espace grâce à la kinect. Les "joints" de tout le corps sont utilisés, à l'exception de ceux des bras. Afin de reconstituer la position des bras, des capteurs inertiels positionnés sur les deux bras et les deux avant bras sont utilisés.

Ceci permet de tracker les bras de la personne, même en cas de superposition (i.e. avec les bras derrière le dos).

J'ai utilisé le (super) projet suivant pour streamer les données de la Kinect : https://github.com/microcosm/KinectV2-OSC
Mon patch est donc prêt à être utilisé avec celui-i, mais libre à vous de modifier l'entrée du patch pour l'adapter au stream voulu.
