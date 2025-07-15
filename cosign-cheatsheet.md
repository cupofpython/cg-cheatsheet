<table>
    <!-- Header -->
    <tr>
        <th>Action</th>
        <th>Example Command</th>
        <th>Tags</th>
        <th>Notes</th>
        <th>Use Cases</th>
    </tr>
    <!-- Start entry in the cheatsheet -->
    <tr>
        <td> <!-- Description -->
        Retrieve an SBOM
        </td>
        <td> <!-- Copy paste command -->
            <pre><code class="language-bash">cosign download attestation \
            --platform=linux/amd64 \
            --predicate-type=https://spdx.dev/Document \
            cgr.dev/chainguard/php | jq -r .payload | base64 -d | jq .predicate
            </code></pre>
        </td>
        <td> <!-- Tags -->
            <ul>
                <li>platform: Architecture</li>
                <li>predicate: Document to download, ex. SBOM, SLSA 1.0 provenance etc.</li>
            </ul>
        </td>
    </tr>
    <!-- End entry in the cheatsheet -->
</table>