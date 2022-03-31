<script>


export default{
    name:"childU",
    data()
    {
        return {
            message :"this is iam said",
        };
    },
methods: {
    sendmessagetoparent()
    {
        this.$emit("my-message",this.message);
    },
},
mounted()
{
    this.sendmessagetoparent();
},
};
</script>
