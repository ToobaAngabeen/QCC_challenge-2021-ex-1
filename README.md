# QCC_challenge-2021-ex-1
Solved exercise 1 of challenge 2021
from qiskit import QuantumRegister, ClassicalRegister, QuantumCircuit
from qiskit import IBMQ, Aer, execute
from math import pi
from ibm_quantum_widgets import CircuitComposer
editorEx = CircuitComposer() 
editorEx
##### Build your quantum circuit here using the composer widget.
# This code is being generated automatically by the IBM Quantum Circuit Composer widget.
# It changes in every update of the widget, so any modifications done in this cell will be lost.
# State: synchronized

from qiskit import QuantumRegister, ClassicalRegister, QuantumCircuit
from numpy import pi

qreg_q = QuantumRegister(3, 'q')
creg_c = ClassicalRegister(3, 'c')
circuit = QuantumCircuit(qreg_q, creg_c)

circuit.rz(pi/2, qreg_q[2])
circuit.sx(qreg_q[2])
circuit.rz(pi/2, qreg_q[2])
circuit.cx(qreg_q[1], qreg_q[2])
circuit.rz(-pi/4, qreg_q[2])
circuit.cx(qreg_q[0], qreg_q[2])
circuit.rz(pi/4, qreg_q[2])
circuit.cx(qreg_q[1], qreg_q[2])
circuit.rz(-pi/4, qreg_q[2])
circuit.cx(qreg_q[0], qreg_q[2])
circuit.rz(pi/4, qreg_q[1])
circuit.rz(pi/4, qreg_q[2])
circuit.cx(qreg_q[0], qreg_q[1])
circuit.rz(pi/2, qreg_q[2])
circuit.rz(pi/4, qreg_q[0])
circuit.rz(-pi/4, qreg_q[1])
circuit.sx(qreg_q[2])
circuit.rz(pi/2, qreg_q[2])
circuit.cx(qreg_q[0], qreg_q[1])
# This code is being generated automatically by the IBM Quantum Circuit Composer widget.
# It changes in every update of the widget, so any modifications done in this cell will be lost.
# State: disconnected

from qiskit import QuantumRegister, ClassicalRegister, QuantumCircuit
from numpy import pi

qreg_q = QuantumRegister(3, 'q')
creg_c = ClassicalRegister(3, 'c')
circuit = QuantumCircuit(qreg_q, creg_c)

circuit.rz(pi/2, qreg_q[2])
circuit.sx(qreg_q[2])
circuit.rz(pi/2, qreg_q[2])
circuit.cx(qreg_q[1], qreg_q[2])
circuit.rz(-pi/4, qreg_q[2])
circuit.cx(qreg_q[0], qreg_q[2])
circuit.rz(pi/4, qreg_q[2])
circuit.cx(qreg_q[1], qreg_q[2])
circuit.tdg(qreg_q[2])
circuit.cx(qreg_q[0], qreg_q[2])
circuit.t(qreg_q[1])
circuit.t(qreg_q[2])
circuit.cx(qreg_q[0], qreg_q[1])
circuit.rz(pi/2, qreg_q[2])
circuit.t(qreg_q[0])
circuit.tdg(qreg_q[1])
circuit.sx(qreg_q[2])
circuit.cx(qreg_q[0], qreg_q[1])
circuit.rz(pi/2, qreg_q[2])
# This code is being generated automatically by the IBM Quantum Circuit Composer widget.
# It changes in every update of the widget, so any modifications done in this cell will be lost.
# State: disconnected

from qiskit import QuantumRegister, ClassicalRegister, QuantumCircuit
from numpy import pi

qreg_q = QuantumRegister(3, 'q')
creg_c = ClassicalRegister(3, 'c')
circuit = QuantumCircuit(qreg_q, creg_c)
circuit.ccx(qreg_q[0], qreg_q[1], qreg_q[2])
# Checking the resulting circuit
qc = editorEx.circuit 
#qc = circuit # Uncomment this line if you want to submit the circuit built using Qiskit code

qc.draw(output='mpl')
#### This is the solution of exercise 1. 
