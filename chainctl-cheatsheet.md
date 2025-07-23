<table>
    <!-- Header -->
    <tr>
        <th>Action</th>
        <th>Example Command</th>
        <th>Flags</th>
        <th>Notes</th>
        <th>Use Cases </th>
    </tr>
    <!-- Start entry in the cheatsheet -->
    <tr>
        <td> <!-- Description -->
        Images diff: compare SBOMs of two Chainguard containers and generates list of packages that have been added/removed. Scans both images and uses itemized CVEs output to create list of vulnerabilities added/removed. 
        </td>
        <td> <!-- Copy paste command -->
            <pre><code class="language-bash">chainctl images diff cgr.dev/chainguard/go:latest cgr.dev/chainguard/go:latest-dev | jq
            </code></pre>
        </td>
        <td> <!-- Flags -->
            <ul>
                <li>N/A</li>
            </ul>
        </td>
        <td> <!-- Notes -->
            <ul>
                <li>Compared in order images are listed</li>
            </ul>
        </td>
        <td> <!-- Use Cases -->
            <ul>
                <li>Compare release version of images</li>
                <li>Trigger rebuilds only on significant changes to a base image</li>
            </ul>
        </td>
    </tr>
    <!-- End entry in the cheatsheet -->
</table>