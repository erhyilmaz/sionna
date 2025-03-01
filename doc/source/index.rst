==================
Sionna
==================
.. include:: <isonum.txt>

Sionna\ |trade| is a `TensorFlow <https://www.tensorflow.org>`_-based open-source library for simulating the physical layer of wireless communication systems.
The rapid prototyping of complex communication system architectures is as simple as connecting the desired building blocks, which are provided as `Keras <https://keras.io>`_ layers.
Using differentiable layers, gradients can be backpropagated through an entire system, which is the key enabler for system optimization and machine learning, especially the integration of neural networks.
NVIDIA GPU acceleration provides orders-of-magnitude faster simulation, enabling the interactive exploration of such systems, for example, in `Jupyter notebooks <https://jupyter.org/>`_ that can be run on cloud services such as `Google Colab <https://colab.research.google.com>`_.
If no GPU is available, Sionna will run on the CPU.

Sionna is developed, continuously extended, and used by NVIDIA to drive 5G and 6G research. It supports MU-MIMO (multi-user multiple input multiple output) link-level simulation setups with 5G-compliant codes including low-density parity check (LDPC) and Polar en-/decoders, the 3GPP channel models, OFDM (orthogonal frequency-division multiplexing), channel estimation, equalization, and soft-demapping. Every building block is an independent module that can be easily tested, understood, and modified according to your needs. The documentation is complete and includes references.


The Benefits of using Sionna
###################################
Most researchers in communications need a tool for link-level simulation to
quickly prototype their ideas and benchmark their algorithms against the
state-of-the-art. However, apart from proprietary software, there existed no
widely-used common open-source tool.
Moreover, experts in one domain, say channel estimation, do not necessarily
have the time or background to evaluate their algorithm for end-to-end performance,
for example, coded bit error rate (BER) over a realistic channel model.

Sionna provides a high-level application programming interface (API) to rapidly model complex communication systems
from end-to-end while allowing you to adapt the part(s) your research
is about. This enables you to focus on your research while making it more
impactful and easily reproducible
by others.

Thanks to `Keras <https://keras.io>`_ and
`TensorFlow <https://www.tensorflow.org>`_, Sionna has native NVIDIA GPU support which makes
it super fast and perfectly suited for machine learning research in communications.


Where to find detailed information?
###################################

.. toctree::
   :maxdepth: 2

   quickstart
   examples/Discover_Sionna.ipynb
   tutorials
   api/sionna

License and Citation
####################
Sionna is Apache-2.0 licensed, as found in the `LICENSE <https://github.com/nvlabs/sionna/blob/main/LICENSE>`_ file.

If you use this software, please cite it as:

.. code:: bibtex

   @article{sionna,
    title = {Sionna: An Open-Source Library for Next-Generation Physical Layer Research},
    author = {Hoydis, Jakob and Cammerer, Sebastian and {Ait Aoudia}, Fayçal and Vem, Avinash and Binder, Nikolaus and Marcus, Guillermo and Keller, Alexander},
    year = {2022},
    month = {Mar.},
    journal = {arXiv preprint},
    online = {https://github.com/NVlabs/sionna/blob/main/sionna.pdf}
   }


