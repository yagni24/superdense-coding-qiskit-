# **superdense-coding-qiskit**

This repository demonstrates the **Superdense Coding** protocol using Qiskit. The project explores how quantum entanglement is used to send two classical bits of information through a single qubit. The quantum circuit uses a Bell state and applies operations to encode and decode the classical bits.

---

# **Superdense Coding Protocol using Qiskit**

This repository contains a quantum circuit built using [Qiskit](https://qiskit.org/) that demonstrates **superdense coding** by encoding two classical bits into one qubit using quantum entanglement. The circuit creates a Bell state, encodes the classical bits, and decodes them using quantum gates.

---

## **Project Description**

In this project, we construct a quantum circuit with:

- **2 qubits** (quantum bits)
- **2 classical bits** (to encode and decode information)

The circuit performs the following operations:

1. **Bell State Creation**: Apply Hadamard (H) gate on qubit 0, followed by a CNOT gate with qubit 0 as control and qubit 1 as target, creating an entangled pair of qubits.
2. **Encoding**: Depending on the classical bits to be sent (00, 01, 10, or 11), apply the corresponding Pauli gates (X, Z) on the sender's qubit.
3. **Decoding**: Apply a CNOT gate and a Hadamard gate on the receiver's qubit to decode the classical bits.
4. **Measurement**: Measure both qubits and store the result in classical bits.

The final state of the qubits is collapsed to either the desired classical bits (00, 01, 10, or 11), showcasing the efficiency of quantum communication.

---

##  **Technologies Used**

- **Python 3.x**
- **Qiskit**
  - `qiskit`
  - `qiskit-aer`
- **Matplotlib** for histogram visualization
- **Jupyter Notebook**

---

## **Output**

The simulation demonstrates the encoding and decoding of classical bits with a single qubit, highlighting the use of entanglement for superdense coding.


## **How to Run**

1. Clone the repository:
   ```bash
   git clone https://github.com/yagni24/superdense-coding-qiskit.git
   cd superdense-coding-qiskit
   ```

2. (Optional) Create a virtual environment:
   ```bash
   python -m venv env
   source env/bin/activate  # On Windows: env\Scripts\activate
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Launch the notebook:
   ```bash
   jupyter notebook
   ```

5. Open and run `superdense_coding_simulation.ipynb`

---
```bash
superdense-coding-qiskit/
│
├── superdense_coding_simulation.ipynb     # Main notebook with quantum circuit for superdense coding
├── requirements.txt                       # Python dependencies
├── .gitignore                             # Git ignore rules
├── README.md                              # Project description and setup instructions
│
└── superdense_images/                     # Folder for all result images
    ├── circuit_result/                    # Contains circuit diagrams
    │   ├── circuit_message_00.png
    │   ├── circuit_message_01.png
    │   ├── circuit_message_10.png
    │   └── circuit_message_11.png
    │
    └── histogram_result/                  # Contains histogram outputs for message decoding
        ├── histogram_message_00.png
        ├── histogram_message_01.png
        ├── histogram_message_10.png
        └── histogram_message_11.png

```

## 📚 **Learn More**

- [Qiskit Documentation](https://qiskit.org/documentation/)
- [Superdense Coding (Qiskit Textbook)](https://qiskit.org/textbook/ch-gates/quantum-communication.html#Superdense-Coding)

---

## 🧑‍💻 **Author**

**Yagni**  
Quantum Computing Enthusiast | Aspiring Research Scientist  
📍 Based in Vadodara

---

