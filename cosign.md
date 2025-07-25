<table>
    <!-- Header -->
    <tr>
        <th>Action</th>
        <th>Example Command</th>
        <th>Flags</th>
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
        <td> <!-- Flags -->
            <ul>
                <li>platform: Architecture</li>
                <li>predicate: Document to download, ex. SBOM, SLSA 1.0 provenance etc.</li>
            </ul>
        </td>
    </tr>
    <!-- End entry in the cheatsheet -->
        <!-- Start entry in the cheatsheet -->
    <tr>
        <td> <!-- Description -->
        Check a signature
        </td>
        <td> <!-- Copy paste command -->
            <pre><code class="language-bash">cosign verify \
            --certificate-oidc-issuer=https://token.actions.githubusercontent.com \
            --certificate-identity=https://github.com/chainguard-images/images/.github/workflows/release.yaml@refs/heads/main \
            cgr.dev/chainguard/redis@sha256:e1f9b716ee5318277060cb6951775aee2bed6733eb93f4a5231945b5f6772727 | jq
            </code></pre>
        </td>
        <td> <!-- Flags -->
            <ul>
                <li></li>
            </ul>
        </td>
    </tr>
    <!-- End entry in the cheatsheet -->
</table>
