<template>
    <skeleton-vue>
        <section id="privacy-section">

            <p>As part of our commitment to protecting your privacy, this statement is designed to provide you with
                information regarding how Meevy,&rdquo; we&rdquo; may use, process, and share the information gathered
                or provided on our app. Information is also collected when you utilize several features from the app.
                This statement applies to all regions.</p>
                <p>&nbsp;</p>

            <h3>YOUR DATA WE USE</h3>
            <p><strong>DATA YOU PROVIDE DIRECTLY TO MEEVY</strong></p>
            <p>Meevy collects personal information about, personal data. Your data is collected when you register on our
                application. The information you provide includes but might not be limited to, email address, first
                name, last name, date of birth as well as any information that is associated with or linked to, or could
                be linked to, any of the foregoing data.</p>
            <p><strong>DEVICE AND LOCATION DATA</strong></p>
            <p>Data concerning the device being used and the location is provided.</p>
            <p><strong>INFORMATION PROVIDED THROUGH YOUR SPOTIFY</strong></p>
            <p>We also collect data from the Spotify service that you provide on login. This includes and is not limited
                to, top artists, top tracks, saved tracks, and your playlists. The processing of this data is connected
                to the application of the app.</p>
            <p><strong>INFORMATION FROM OTHER SOURCES</strong></p>
            <p>We also obtain information from other sources that might be used during the app operation and combine it
                with the information we collect from you directly.</p>
            <h3>HOW WE USE YOUR DATA AND THE LAWFUL BASIS FOR SUCH PROCESSING</h3>
            <p>We use your information mainly to deliver and improve our services. Additionally, provide more services
                that might be relevant to you. Your data is processed on the following bases:</p>
            <ol>
                <li>Administer your account and provide our services to you</li>
                <li>Help you connect with other users by recommending and showing profiles to one another</li>
                <li>To improve our services provided to you</li>
                <li>Administer relevant campaigns</li>
                <li>Ensure legal compliance</li>
                <li>Detect unauthorized activities</li>
            </ol>
            <p>To process your information as described in this privacy policy, we rely on the following legal bases:
            </p>
            <ol>
                <li>Provide our services to you &ndash; the reason we process your information for the above purposes is
                    to perform the contract you have with us. For example, as you go about using the service to build
                    connections and other authorized relevant reasons, you use the information to maintain your profile,
                    make it viewable, and recommend other members. Also, provide free and paid features</li>
                <li>Legitimate interest &ndash; We process some of the information based on our legitimate interest to
                    promote our services, keep other members safe and defend ourselves in legal action</li>
            </ol>
            <ul>
                <li><em>Consent:</em> If you choose to provide us with information that may be considered
                    &ldquo;special&rdquo; or &ldquo;sensitive&rdquo; in certain jurisdictions, such as your sexual
                    orientation, you&rsquo;re consenting to our processing of that information by this Privacy Policy.
                    From time to time, we may ask for your consent to collect specific information such as your precise
                    geolocation, or use your information for certain specific reasons. In some cases, you may withdraw
                    your consent by adapting your settings (for instance about the collection of our precise
                    geolocation) or by deleting your content (for instance where you entered information in your profile
                    that may be considered &ldquo;special&rdquo; or &ldquo;sensitive&rdquo;). In any case, you may
                    withdraw your consent at any time by contacting us at the address provided at the end of this
                    Privacy Policy.</li>
            </ul>
            <h3>HOW WE SHARE INFORMATION</h3>
            <p>Our goal is to build meaningful connections based on music data. The main sharing of information is with
                other members of the application. For instance, your top artists and tracks may be shared with other
                members. Other third parties necessary for the operation and improvement of the services might have
                access to the information. Such services include hosting, maintenance, analytics, and security
                operations. We may disclose the information if it is reasonably and legally necessary to do so for
                example to comply with a court order.</p>
            <p>We may ask for your consent to share information with third parties. In any such case, we will make it
                clear why we want the information.</p>
            <h3>RETAINING AND DELETING YOUR DATA</h3>
            <p>Meevy will only retain your data for the duration necessary. You can choose to delete your data via the
                delete account option in the app settings</p>
            <h3>YOUR RIGHTS</h3>
            <p>Access/ Update tools in the service &ndash; tools in the application can help you access your personal
                information that is provided to us and delete it.</p>
            <p>Device Permissions &ndash; Mobile platforms can have permission systems for specific device data and
                notification types. You can change your device settings to either consent to or oppose the collection or
                processing of given notifications</p>
            <p>Uninstall &ndash; you can stop all information collection by uninstalling the app through the standard
                uninstall process for your device. NOTE: uninstalling the app does not close the app</p>
        </section>

    </skeleton-vue>
</template>

<script>
import SkeletonVue from '../components/Skeleton.vue';
export default {
    name: 'privacy-policy',
    components: {
        SkeletonVue
    }

}
</script>
<style scoped>
section {
    min-height: 100vh;
    padding: 2em 0;
    font-size: smaller;
    line-height: 3;
    margin-top: 2em;
    color: rgb(27, 27, 27);
}
li{
    list-style: lower-alpha;
}
ol{
    margin-left: 3em;
}

</style>