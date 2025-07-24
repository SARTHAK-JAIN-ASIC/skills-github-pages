
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sarthak Jain - Hardware Engineering Portfolio</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        pre {
            background-color: #f4f4f4;
            padding: 10px;
            border-radius: 5px;
            overflow-x: auto;
        }
    </style>
</head>
<body class="bg-gray-100 font-sans">
    <header class="bg-blue-600 text-white text-center py-8">
        <h1 class="text-4xl font-bold">Sarthak Jain</h1>
        <p class="text-xl">USC EE MS 2025 | FPGA Design Engineer | Computer Architecture</p>
        <p class="mt-2">
            <a href="https://github.com/SARTHAK-JAIN-ASIC" class="text-white underline">GitHub</a> | 
            <a href="https://linkedin.com/in/sarthak-jain-asic" class="text-white underline">LinkedIn</a> | 
            <a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="9ceffdeee8f4fdf7dce9efffb2f9f8e9">[email&#160;protected]</a>
        </p>
    </header>
    <section class="max-w-4xl mx-auto my-8">
        <h2 class="text-3xl font-bold mb-4">Portfolio</h2>
        <p class="mb-4">All projects are hosted in my <a href="https://github.com/SARTHAK-JAIN-ASIC/EE533" class="text-blue-600 underline">EE533 repository</a>.</p>
        <div class="grid grid-cols-1 gap-6">
            <div class="bg-white p-6 rounded-lg shadow-md">
                <h3 class="text-2xl font-semibold">AI-Accelerated Network Traffic Classifier</h3>
                <p class="mt-2">Designed an AI-driven classifier on Xilinx NetFPGA using SystemVerilog and Python-trained neural networks (NSL-KDD dataset). Achieved 25% throughput improvement.</p>
                <p class="mt-2"><strong>Tools:</strong> SystemVerilog, Vivado, Python, NetFPGA</p>
                <p class="mt-2"><strong>Results:</strong> Improved classification throughput by 25%, reduced FPGA resource utilization by 10%.</p>
                <p class="mt-2">
                    <a href="https://github.com/SARTHAK-JAIN-ASIC/EE533/tree/main/network-classifier" class="text-blue-600 underline">Project Folder</a> | 
                    <a href="https://drive.google.com/your-network-presentation-link" class="text-blue-600 underline">Presentation</a>
                </p>
                <p class="mt-2"><strong>Code Snippet (Python - NSL-KDD Preprocessing):</strong></p>
                <pre><code>from sklearn.ensemble import RandomForestClassifier
from sklearn.preprocessing import StandardScaler
import numpy as np

# Feature selection using Random Forest
rf = RandomForestClassifier()
rf.fit(X_train, y_train)
top_features = np.argsort(rf.feature_importances_)[-10:]
X_train_selected = X_train[:, top_features]</code></pre>
                <img src="network_classifier_diagram.png" alt="Network Classifier Diagram" class="mt-4 w-full rounded">
            </div>
            <div class="bg-white p-6 rounded-lg shadow-md">
                <h3 class="text-2xl font-semibold">GPGPU Microarchitecture Design</h3>
                <p class="mt-2">Modeled a GPGPU pipeline in GEM5, optimizing thread scheduling for 20% performance gain. Focused on microarchitecture design and simulation.</p>
                <p class="mt-2"><strong>Tools:</strong> GEM5, Python, C++</p>
                <p class="mt-2"><strong>Results:</strong> Achieved 20% performance improvement in thread scheduling.</p>
                <p class="mt-2">
                    <a href="https://github.com/SARTHAK-JAIN-ASIC/EE533/tree/main/gpgpu-microarchitecture" class="text-blue-600 underline">Project Folder</a> | 
                    <a href="https://drive.google.com/your-gpgpu-presentation-link" class="text-blue-600 underline">Presentation</a>
                </p>
                <p class="mt-2"><strong>Code Snippet (Pseudocode - Thread Scheduling):</strong></p>
                <pre><code>function schedule_threads():
    for warp in warps:
        if warp.ready:
            issue_instructions(warp)
            update_pipeline_state()
    return performance_metrics</code></pre>
                <img src="gpgpu_diagram.png" alt="GPGPU Pipeline Diagram" class="mt-4 w-full rounded">
            </div>
            <div class="bg-white p-6 rounded-lg shadow-md">
                <h3 class="text-2xl font-semibold">PCIe Gen 3 Simulation</h3>
                <p class="mt-2">Designed and verified PCIe Gen 3 interface in SystemVerilog, reducing transaction latency by 15%. Focused on high-speed interface design.</p>
                <p class="mt-2"><strong>Tools:</strong> SystemVerilog, Vivado</p>
                <p class="mt-2"><strong>Results:</strong> Reduced transaction latency by 15%.</p>
                <p class="mt-2">
                    <a href="https://github.com/SARTHAK-JAIN-ASIC/EE533/tree/main/pcie-gen3" class="text-blue-600 underline">Project Folder</a> | 
                    <a href="https://drive.google.com/your-pcie-presentation-link" class="text-blue-600 underline">Presentation</a>
                </p>
                <p class="mt-2"><strong>Code Snippet (SystemVerilog - PCIe Interface):</strong></p>
                <pre><code>module pcie_gen3_if (
    input logic clk,
    input logic rst_n,
    output logic [63:0] data_out
);
    always @(posedge clk or negedge rst_n) begin
        if (!rst_n) data_out <= 64'b0;
        else data_out <= // Transaction processing
    end
endmodule</code></pre>
                <img src="pcie_diagram.png" alt="PCIe Gen 3 Diagram" class="mt-4 w-full rounded">
            </div>
            <div class="bg-white p-6 rounded-lg shadow-md">
                <h3 class="text-2xl font-semibold">ARMv7 Pipelined CPU</h3>
                <p class="mt-2">Implemented a pipelined ARMv7 CPU in Verilog, optimizing for performance and resource efficiency.</p>
                <p class="mt-2"><strong>Tools:</strong> Verilog, Vivado</p>
                <p class="mt-2"><strong>Results:</strong> Achieved efficient pipeline with minimal stalls.</p>
                <p class="mt-2">
                    <a href="https://github.com/SARTHAK-JAIN-ASIC/EE533/tree/main/armv7-cpu" class="text-blue-600 underline">Project Folder</a> | 
                    <a href="https://drive.google.com/your-armv7-presentation-link" class="text-blue-600 underline">Presentation</a>
                </p>
                <p class="mt-2"><strong>Code Snippet (Verilog - Pipeline Stage):</strong></p>
                <pre><code>module pipeline_stage (
    input logic clk,
    input logic [31:0] instr_in,
    output logic [31:0] instr_out
);
    always @(posedge clk) begin
        instr_out <= instr_in;
    end
endmodule</code></pre>
                <img src="armv7_diagram.png" alt="ARMv7 Pipeline Diagram" class="mt-4 w-full rounded">
            </div>
        </div>
    </section>
<script data-cfasync="false" src="/cdn-cgi/scripts/5c5dd728/cloudflare-static/email-decode.min.js"></script><script>(function(){function c(){var b=a.contentDocument||a.contentWindow.document;if(b){var d=b.createElement('script');d.innerHTML="window.__CF$cv$params={r:'9642e09ee9732ec3',t:'MTc1MzM1NDQ0NC4wMDAwMDA='};var a=document.createElement('script');a.nonce='';a.src='/cdn-cgi/challenge-platform/scripts/jsd/main.js';document.getElementsByTagName('head')[0].appendChild(a);";b.getElementsByTagName('head')[0].appendChild(d)}}if(document.body){var a=document.createElement('iframe');a.height=1;a.width=1;a.style.position='absolute';a.style.top=0;a.style.left=0;a.style.border='none';a.style.visibility='hidden';document.body.appendChild(a);if('loading'!==document.readyState)c();else if(window.addEventListener)document.addEventListener('DOMContentLoaded',c);else{var e=document.onreadystatechange||function(){};document.onreadystatechange=function(b){e(b);'loading'!==document.readyState&&(document.onreadystatechange=e,c())}}}})();</script></body>
</html>
